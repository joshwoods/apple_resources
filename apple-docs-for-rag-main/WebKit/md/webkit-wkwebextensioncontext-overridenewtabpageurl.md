

- WebKit
- WKWebExtensionContext
-  overrideNewTabPageURL 

Instance Property

# overrideNewTabPageURL

The URL to use as an alternative to the default new tab page, if the extension has one.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var overrideNewTabPageURL: URL? { get }
```

## Discussion

Provides the URL for a new tab page, if provided by the extension; otherwise `nil` if no page is defined.

The app should prompt the user for permission to use the extension’s new tab page as the default.

Note

Navigation to the override new tab page is only possible after this extension has been loaded.

## See Also

### Related Documentation

var webViewConfiguration: WKWebViewConfiguration?

The web view configuration to use for web views that load pages from this extension.

