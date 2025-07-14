

- WebKit
- WKWebView
-  mediaType 

Instance Property

# mediaType

The media type for the contents of the web view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
var mediaType: String? { get set }
```

## Discussion

When the value of this property is `nil`, the web view derives the current media type from the CSS media property of its content. If you assign a value other than `nil` to this property, the web view uses the value you provide instead. The default value of this property is `nil`.

## See Also

### Inspecting the view information

var scrollView: UIScrollView

The scroll view associated with the web view.

var title: String?

The page title.

var url: URL?

The URL for the current webpage.

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

