

- WebKit
- WKWebView
-  navigationDelegate 

Instance Property

# navigationDelegate

The object you use to manage navigation behavior for the web view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
weak var navigationDelegate: (any WKNavigationDelegate)? { get set }
```

## Discussion

Provide a delegate object when you want to manage or restrict navigation in your web content, track the progress of navigation requests, and handle authentication challenges for any new content. The object you specify must conform to the WKNavigationDelegate protocol.

## See Also

### Managing navigation between webpages

protocol WKNavigationDelegate

Methods for accepting or rejecting navigation changes, and for tracking the progress of navigation requests.

