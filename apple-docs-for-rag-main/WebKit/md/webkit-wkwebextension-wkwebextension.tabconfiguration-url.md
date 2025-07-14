

- WebKit
- WKWebExtension
- WKWebExtension.TabConfiguration
-  url 

Instance Property

# url

Indicates the initial URL for the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var url: URL? { get }
```

## Discussion

If this property is `nil`, the app’s default start page should appear in the tab.

