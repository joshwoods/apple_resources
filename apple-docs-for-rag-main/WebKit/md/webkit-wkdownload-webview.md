

- WebKit
- WKDownload
-  webView 

Instance Property

# webView

The web view where the download initiated.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
weak var webView: WKWebView? { get }
```

## See Also

### Inspecting the download

var originalRequest: URLRequest?

An object that represents the request that initiated the download.

