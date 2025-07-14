

- WebKit
- WKWebView
-  hasOnlySecureContent 

Instance Property

# hasOnlySecureContent

A Boolean value that indicates whether the web view loaded all resources on the page through securely encrypted connections.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var hasOnlySecureContent: Bool { get }
```

## Discussion

WKWebView is key-value observing (KVO) compliant for this property.

## See Also

### Inspecting the view information

var scrollView: UIScrollView

The scroll view associated with the web view.

var title: String?

The page title.

var url: URL?

The URL for the current webpage.

var mediaType: String?

The media type for the contents of the web view.

var customUserAgent: String?

The custom user agent string.

var serverTrust: SecTrust?

The trust management object you use to evaluate trust for the current webpage.

var themeColor: UIColor?

The theme color that the system gets from the first valid meta tag in the webpage.

var underPageBackgroundColor: UIColor!

The color the web view displays behind the active page, visible when the user scrolls beyond the bounds of the page.

