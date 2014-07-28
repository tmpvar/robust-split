# robust-split

Use this package when you want to split a double precision floating point number into a 2-part robust geometric predicate.

Why would you ever want to do that? Well, robust geometric predicates are an efficient way to perform
_exact_ mathmatical operations on javascript numbers.

# install

```npm install robust-split``

# use

```javascript

var rsplit = require('robust-split');

var p = rsplit(0.3);

console.log(p); //[ 2.980232227667301e-9,
                //  0.29999999701976776 ]
```

You could then pass the robust predicate into a `[robust-estimate-float](https://github.com/tmpvar/robust-estimate-float)`

```
var num = require('robust-estimate-float');

var r = num(p);

console.log(r) // 0.3
```

See the rest of the [robust family of packages](http://npmsearch.com/?q=keywords:robust)

# credits

This code is pulled from Mikola Lysenko's [Robust arithmetic in JavaScript](https://github.com/mikolalysenko/robust-arithmetic-notes) class notes.

