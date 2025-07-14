

- WebKit
- WKWebExtension
- WKWebExtension.WindowConfiguration
-  tabURLs 

Instance Property

# tabURLs

Indicates the URLs that the window should initially load as tabs.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var tabURLs: [URL] { get }
```

## Discussion

If tabURLs and tabs are both empty, the app’s default start page should appear in a tab.

## See Also

### Related Documentation

var tabs: [any WKWebExtensionTab]

Indicates the existing tabs that should be moved to the window.

