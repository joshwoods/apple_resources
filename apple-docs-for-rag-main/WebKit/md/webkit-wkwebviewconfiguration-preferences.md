

- WebKit
- WKWebViewConfiguration
-  preferences 

Instance Property

# preferences

The object that manages the preference-related settings for the web view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var preferences: WKPreferences { get set }
```

## Discussion

Use the preferences object in this property to customize the rendering, JavaScript, and other preferences related to your web view. You can also change the preferences by assigning a new WKPreferences object to this property.

## See Also

### Configuring the web view’s preferences

var defaultWebpagePreferences: WKWebpagePreferences!

The default preferences to use when loading and rendering content.

