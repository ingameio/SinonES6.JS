# SinonES6.JS
Sinon.js version compatible with ES6.
Everything is like the original version of [sinon](http://github.com/cjohansen/Sinon.JS), plus generators mocking.
``` js
var sinon = require('sinon-es6');

var objectToMock = {
    generator: function* (a, b) { yield ... }
};

sinon.mock(objectToMock).expects('generator').withArgs(2,3).returns(6);
```

All credits to @cjohansen and [Sinon.JS](http://github.com/cjohansen/Sinon.JS) contributors.
