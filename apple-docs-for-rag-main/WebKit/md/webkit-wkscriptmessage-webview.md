

- WebKit
- WKScriptMessage
-  webView 

Instance Property

# webView

The web view that sent the message.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
weak var webView: WKWebView? { get }
```

## See Also

### Getting Message-Related Information

var frameInfo: WKFrameInfo

The frame that sent the message.

var world: WKContentWorld

The namespace in which the JavaScript code executes.

