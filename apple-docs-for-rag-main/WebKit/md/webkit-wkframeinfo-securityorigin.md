

- WebKit
- WKFrameInfo
-  securityOrigin 

Instance Property

# securityOrigin

The frame’s security origin.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
var securityOrigin: WKSecurityOrigin { get }
```

## Discussion

The WKSecurityOrigin object consists of a host name, a protocol, and a port number.

## See Also

### Inspecting frame information

var isMainFrame: Bool

A Boolean value indicating whether the frame is the web site’s main frame or a subframe.

var request: URLRequest

The frame’s current request.

var webView: WKWebView?

The web view that contains this frame and the containing webpage.

