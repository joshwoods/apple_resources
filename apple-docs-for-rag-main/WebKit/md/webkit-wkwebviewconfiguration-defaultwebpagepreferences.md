

- WebKit
- WKWebViewConfiguration
-  defaultWebpagePreferences 

Instance Property

# defaultWebpagePreferences

The default preferences to use when loading and rendering content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
@NSCopying @MainActor
var defaultWebpagePreferences: WKWebpagePreferences! { get set }
```

## Discussion

Use this property to specify the JavaScript settings and content mode for new webpages. When the web view navigates to a new page, it passes the default preferences to its navigation delegate, which can modify the preferences or pass them as they are.

## See Also

### Configuring the web view’s preferences

var preferences: WKPreferences

The object that manages the preference-related settings for the web view.

