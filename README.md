jquery-include
==============

A simple way to include html using jQuery and AJAX

Usage
=====

1.include jquery and jquery.include.js
```html
<script src="http://code.jquery.com/jquery-1.11.2.min.js"></script>
<script src="./jquery.include.js"></script>
```

2.add `<div class="include" data-path="path/to/load.html"></div>` to the location you want include html from other files.

3.activate the include function
```javaScript
	var domScript = ['one.js', 'two.js'];
	$.include(domScript);
```

**You can download the whole repository and check the index.html for detail**

Attention
=========
Because this plugin is **USING AJAX**, so you need to put your project on server to test it. The variable `domScript` is other js file that mainipulate DOM. As you know if you using AJAX to load some DOM to document, the event listener bind to them before won't work.
