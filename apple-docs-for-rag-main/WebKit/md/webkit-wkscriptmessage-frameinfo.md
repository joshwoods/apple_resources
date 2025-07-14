

- WebKit
- WKScriptMessage
-  frameInfo 

Instance Property

# frameInfo

The frame that sent the message.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@NSCopying @MainActor
var frameInfo: WKFrameInfo { get }
```

## See Also

### Getting Message-Related Information

var webView: WKWebView?

The web view that sent the message.

var world: WKContentWorld

The namespace in which the JavaScript code executes.

