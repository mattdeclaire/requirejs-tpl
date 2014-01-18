requirejs-tpl
=============

Plugin for RequireJS for loading template files via requirejs-text

# Requirements

 - [RequireJS](http://requirejs.org/)
 - [require-text](https://github.com/requirejs/text)
 - [jQuery](http://jquery.com/)

# Assumptions

 - templates must be available via same domain, in `/templates`
 - template files use the `.tpl` extension

# Usage

`/templates/hello.tpl`
```
<p>Hello World.</p>
```

```js
define(['tpl!hello'], function(tpl) {
	document.write(tpl);
});
```