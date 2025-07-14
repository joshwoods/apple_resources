

- WebKit
- WKWebExtension
- WKWebExtension.WindowConfiguration
-  tabs 

Instance Property

# tabs

Indicates the existing tabs that should be moved to the window.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var tabs: [any WKWebExtensionTab] { get }
```

## Discussion

If tabs and tabURLs are both empty, the app’s default start page should appear in a tab.

## See Also

### Related Documentation

var tabURLs: [URL]

Indicates the URLs that the window should initially load as tabs.

