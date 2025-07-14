

- WebKit
- WKWebpagePreferences
-  preferredContentMode 

Instance Property

# preferredContentMode

The content mode for the web view to use when it loads and renders a webpage.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
@MainActor
var preferredContentMode: WKWebpagePreferences.ContentMode { get set }
```

## Discussion

The default value of this property is WKWebpagePreferences.ContentMode.recommended. The web view ignores this preference for subframe navigation.

## See Also

### Setting the preferred content mode

enum ContentMode

Constants that indicate how to render web view content.

