

- WebKit JS
- StyleMedia
-  matchMedium 

Instance Method

# matchMedium

Evaluates the given string as a media query and returns the result.

Safari Desktop 5.0+Safari Mobile 4.2+

``` source
boolean matchMedium(
    optional DOMString mediaquery
);
```

## Parameters 

`mediaquery`  

The media query to evaluate.

## Return Value

`true` if the media query is logically true; otherwise, `false`.

## Discussion

For example, `window.styleMedia.matchMedium("(color)")` returns `true` if the display device is a color device. You can also use this method to check whether the browser supports 3D transforms as follows:

if (&#39;styleMedia&#39; in window &amp;&amp; window.styleMedia.matchMedium(&quot;(-webkit-transform-3d)&quot;)) {
  // Insert 3D code here
}

Or check to see whether the browser supports animations as follows:

if (&#39;styleMedia&#39; in window &amp;&amp; window.styleMedia.matchMedium(&quot;(-webkit-animation)&quot;)) {
  // Insert animation code here
}

