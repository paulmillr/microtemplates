# Javascript micro-templates

aka underscore templates. No dependencies, no bullshit, pure functionality.

Original code and idea [by John Resig](http://ejohn.org/blog/javascript-micro-templating/). With source URL support.

For browsers and node.js.

## Installation
* Just include microtemplates before your scripts.
* `npm install microtemplates` if you’re using node.js.
* `component install paulmillr/microtemplates` if you’re using [component(1)](https://github.com/component/component).
* `bower install microtemplates` if you’re using [Twitter Bower](http://bower.io).

## Usage

* `microtemplate(string)` generates function
* the function tooks one optional argument (object) and generates string

Node.js:

```javascript
var microtemplates = require('microtemplates');
var fn = microtemplates('Hello, <%= name %>');
fn({name: 'Paul'});
```

Browser:

```javascript
// component(1)
var microtemplate = require('microtemplates');
microtemplates('Hello, <%= name %>')({name: 'Paul'});

// Default:
window.microtemplate('Hello, <%= name %>')({name: 'Paul'});
```

## License

The MIT License (MIT)

Copyright (c) 2013 Paul Miller (http://paulmillr.com/)
Copyright (c) 2008 John Resig (http://ejohn.org/)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
