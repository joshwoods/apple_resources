

- WebKit
- WKWebExtension
- WKWebExtension.TabConfiguration
-  parentTab 

Instance Property

# parentTab

Indicates the parent tab with which the tab should be related.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var parentTab: (any WKWebExtensionTab)? { get }
```

## Discussion

If this property is `nil`, no parent tab was specified.

