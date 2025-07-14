

- WebKit
- WKWebExtensionContext
-  optionsPageURL 

Instance Property

# optionsPageURL

The URL of the extension’s options page, if the extension has one.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var optionsPageURL: URL? { get }
```

## Discussion

Provides the URL for the dedicated options page, if provided by the extension; otherwise `nil` if no page is defined.

The app should provide access to this page through a user interface element.

Note

Navigation to the options page is only possible after this extension has been loaded.

## See Also

### Related Documentation

var webViewConfiguration: WKWebViewConfiguration?

The web view configuration to use for web views that load pages from this extension.

