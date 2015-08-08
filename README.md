#k-flash

This is similar to [connect-flash](https://github.com/jaredhanson/connect-flash) but for [kantele](https://github.com/kantele/kantele). 

k-flash should work along connect-flash; the messages from connect-flash will be accessible from this module.

![image](https://cloud.githubusercontent.com/assets/433707/4265716/454049a8-3c5c-11e4-9c0a-9eb06539ed0a.png)


##Demo

https://derby-demos.herokuapp.com/derby-flash

##Requirements

- [Node.js](http://nodejs.org)
- [kantele](https://github.com/kantele/kantele)


##Installation

`npm install k-flash`

##Usage

###Initialization

```javascript
app.use(require('k-flash'))
```

k-flash also accepts an `options` object:

```javascript
app.component(require('k-flash'), { useToast: true })
```

Currently the supported options are:

- **useToast: boolean**
	use [k-toast](https://github.com/k-components/k-toast) to show the messages, if available.

###CSS

This serves as an example stylesheet, import this from `index.styl` to use it. 
```css
@import '../../node_modules/k-flash'
```

###In templates

```html
<view name="k-flash"></view>
```

###Adding messages

```javascript
model.flash('error', 'An error happened!');

```

##License

(The MIT License)

Copyright (c) 2013-2014 Ilkka Huotari

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
