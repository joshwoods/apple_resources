

- WebKit
- WKFrameInfo
-  webView 

Instance Property

# webView

The web view that contains this frame and the containing webpage.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
weak var webView: WKWebView? { get }
```

## See Also

### Inspecting frame information

var isMainFrame: Bool

A Boolean value indicating whether the frame is the web site’s main frame or a subframe.

var request: URLRequest

The frame’s current request.

var securityOrigin: WKSecurityOrigin

The frame’s security origin.

