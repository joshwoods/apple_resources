

- WebKit
- WKWebView
-  url 

Instance Property

# url

The URL for the current webpage.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var url: URL? { get }
```

## Discussion

This property contains the URL for the webpage that the web view currently displays. Use this URL in places where you reflect the webpage address in your app’s user interface.

WKWebView is key-value observing (KVO) compliant for this property.

## See Also

### Inspecting the view information

var scrollView: UIScrollView

The scroll view associated with the web view.

var title: String?

The page title.

var mediaType: String?

The media type for the contents of the web view.

var customUserAgent: String?

The custom user agent string.

var serverTrust: SecTrust?

The trust management object you use to evaluate trust for the current webpage.

var hasOnlySecureContent: Bool

A Boolean value that indicates whether the web view loaded all resources on the page through securely encrypted connections.

var themeColor: UIColor?

The theme color that the system gets from the first valid meta tag in the webpage.

var underPageBackgroundColor: UIColor!

The color the web view displays behind the active page, visible when the user scrolls beyond the bounds of the page.

