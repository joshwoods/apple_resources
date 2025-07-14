

- WebKit
- WebFrame
-  childFrames Deprecated

Instance Property

# childFrames

The frames of the web frame’s immediate children.

macOS 10.3–10.14Deprecated

``` source
var childFrames: [Any]! { get }
```

## Discussion

Each child web frame is an instance of `WebFrame` and corresponds to an HTML frameset or `iframe` element.

## See Also

### Getting Related Frames and Views

var parent: WebFrame!

The web frame’s parent web frame.

Deprecated

var frameView: WebFrameView!

The web frame’s view object.

Deprecated

var webView: WebView!

The view object that manages the web frame.

Deprecated

