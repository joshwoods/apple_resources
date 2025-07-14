

- WebKit
- WKWebView
-  customUserAgent 

Instance Property

# customUserAgent

The custom user agent string.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
var customUserAgent: String? { get set }
```

## Discussion

Use this property to specify a custom user agent string for your web view. The default value of this property is `nil`.

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

var serverTrust: SecTrust?

The trust management object you use to evaluate trust for the current webpage.

var hasOnlySecureContent: Bool

A Boolean value that indicates whether the web view loaded all resources on the page through securely encrypted connections.

var themeColor: UIColor?

The theme color that the system gets from the first valid meta tag in the webpage.

var underPageBackgroundColor: UIColor!

The color the web view displays behind the active page, visible when the user scrolls beyond the bounds of the page.

