##Class

example

    var L = new lettuce();
    var zero = function(){
    
    };
    var sub = new L.Class(zero);

##Template

example

    var L = new lettuce();
    var data = {
        "title": "JavaScript Templates"
    };

    var result = L.tmpl("<h3>{%=o.title%}</h3>\n!@#$%^&*()-=", data);

##Router

Example

    var L = new lettuce();
    
    var check = L.Router
                .add(/#about/,log)
                .add(/#what/, log)
                .add(/#why/, log)
                .load();;

##Promise

example

    function late(n) {
        var L = new lettuce();
        var p = new L.Promise();
        return p;
    }

    late(100).then(
    ).then(
    ).done();

##Ajax

example

    lettuce.get('/bower.json', function(result){
        equal(result["name"], "lettuce");
        done();
    })
