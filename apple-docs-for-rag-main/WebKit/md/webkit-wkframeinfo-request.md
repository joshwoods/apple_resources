

- WebKit
- WKFrameInfo
-  request 

Instance Property

# request

The frame’s current request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var request: URLRequest { get }
```

## See Also

### Inspecting frame information

var isMainFrame: Bool

A Boolean value indicating whether the frame is the web site’s main frame or a subframe.

var securityOrigin: WKSecurityOrigin

The frame’s security origin.

var webView: WKWebView?

The web view that contains this frame and the containing webpage.

