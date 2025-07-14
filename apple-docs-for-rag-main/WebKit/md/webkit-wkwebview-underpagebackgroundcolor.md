

- WebKit
- WKWebView
-  underPageBackgroundColor 

Instance Property

# underPageBackgroundColor

The color the web view displays behind the active page, visible when the user scrolls beyond the bounds of the page.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@NSCopying @MainActor
var underPageBackgroundColor: UIColor! { get set }
```

**macOS**

``` source
@NSCopying @MainActor
var underPageBackgroundColor: NSColor! { get set }
```

## Discussion

The web view derives the default value of this property from the content of the page, using the background colors of the `` and `` elements with the background color of the web view. To override the default color, set this property to a new color.

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

var themeColor: UIColor?

The theme color that the system gets from the first valid meta tag in the webpage.

