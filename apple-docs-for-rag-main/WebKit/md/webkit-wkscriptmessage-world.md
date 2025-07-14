

- WebKit
- WKScriptMessage
-  world 

Instance Property

# world

The namespace in which the JavaScript code executes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
var world: WKContentWorld { get }
```

## Discussion

For more information about content worlds, see WKContentWorld.

## See Also

### Getting Message-Related Information

var frameInfo: WKFrameInfo

The frame that sent the message.

var webView: WKWebView?

The web view that sent the message.

