defaultdict
-----------

Nodejs port of python [defaultdict](http://docs.python.org/2/library/collections.html#collections.defaultdict)

examples
--------

```javascript
var DefaultDict = require('defaultdict')

// create dict
var dict = new DefaultDict(0);

// works like normal dict
dict.set('foo', 'bar');
dict.get('foo');
//=> 'bar'

// get undefined keys
dict.get('qux');
//=> 0

// add a value to a key (must support + operator)
dict.add('qux', 5);
dict.get('qux')
//=> 5
```
