# JAVASCRIPT LIBRARIES
JavaScript library is a library of pre-written JavaScript which allows for easier development of JavaScript-based applications, especially for AJAX and other web-centric technologies.


Some examples are listed below:
## Howler.js

![alt text](https://github.com/marc-acm/jslibrary/blob/master/howler.png)

An audio library which defaults to Web Audio API and falls back to HTML5 Audio making audio in JavaScript easy
and reliable across all platforms.

SAMPLE CODE:
```sh
<script src="/path/to/howler.js"></script>
<script>
    var sound = new Howl({
      src: ['sound.webm', 'sound.mp3']
    });
</script>

```

Control multiple sounds:
```sh
var sound = new Howl({
  src: ['sound.webm', 'sound.mp3']
});

// Play returns a unique Sound ID that can be passed
// into any method on Howl to control that specific sound.
var id1 = sound.play();
var id2 = sound.play();

// Fade out the first sound and speed up the second.
sound.fade(1, 0, 1000, id1);
sound.rate(1.5, id2);

````

 
## Highlight.js

Highlight.js is a syntax highlighter written in JavaScript. It works in the browser as well as on the server. 
It works with pretty much any markup, doesn’t depend on any framework and has automatic language detection.
![alt text](https://github.com/marc-acm/jslibrary/blob/master/highlightjs.png)

SAMPLE CODE:
To use highlight.js on a web page you must link the library along with one of the styles and calling 
initHighlightingOnLoad:

```sh
<link rel="stylesheet" href="/path/to/styles/default.css">
<script src="/path/to/highlight.pack.js"></script>
<script>hljs.initHighlightingOnLoad();</script>
```

This will find and highlight code inside of pre-code tags; it tries to detect the language automatically. 
If automatic detection doesn’t work for you, you can specify the language in the class attribute:

```sh

<pre><code> class="html">...</code></pre>

```

The list of supported language classes is available in the class reference. Classes can also be prefixed with 
either language- or lang-.To disable highlighting altogether use the nohighlight class:


```sh

<pre><code class="nohighlight">...</code></pre>

```




## Dragula.js

A JavaScript library that provides drag and drop functionality on DOM elements.
![alt text](https://github.com/marc-acm/jslibrary/blob/master/dragula.png)

Usage
Dragula provides the easiest possible API to make drag and drop a breeze in your applications.

SAMPLE CODE:
The example below allows the user to drag elements from left into right, and from right into left.

```sh
dragula([document.querySelector('#left'), 
document.querySelector('#right')]);
```




## Difference Between A Library and A Framework

The main difference between a library and a framework is "Inversion of Control".
A library is a ready-made which can be used methods in your application while framework is more like an architecture where 
there is a set or a structure that needs to be followed.

