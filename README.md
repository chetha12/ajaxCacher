ajaxCacher
==========

Extends jQuery's ajax function to ensure fetches from the server is cached by storing data in a variable rather than just afixing a timestamp to the URL.

## Usage

Usage is the same as jQuery's ajax function, but calling ajaxCacher instead:

```
$.ajaxCacher({
  url: "getsomething.php",
  cache: true
})
```

In this case however, the cache option will instruct the ajaxCacher to look in the local variable rather than use a timestamp to hope the browser will provide caching (not always guaranteed)
