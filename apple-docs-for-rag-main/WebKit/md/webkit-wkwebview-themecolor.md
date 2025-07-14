

- WebKit
- WKWebView
-  themeColor 

Instance Property

# themeColor

The theme color that the system gets from the first valid meta tag in the webpage.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
var themeColor: UIColor? { get }
```

**macOS**

``` source
@MainActor
var themeColor: NSColor? { get }
```

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

var hasOnlySecureContent: Bool

A Boolean value that indicates whether the web view loaded all resources on the page through securely encrypted connections.

var underPageBackgroundColor: UIColor!

The color the web view displays behind the active page, visible when the user scrolls beyond the bounds of the page.

