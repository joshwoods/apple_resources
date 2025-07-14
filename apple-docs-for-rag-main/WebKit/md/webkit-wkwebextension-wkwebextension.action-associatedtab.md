

- WebKit
- WKWebExtension
- WKWebExtension.Action
-  associatedTab 

Instance Property

# associatedTab

The tab that this action is associated with, or `nil` if it’s the default action.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
weak var associatedTab: (any WKWebExtensionTab)? { get }
```

## Discussion

When this property is `nil`, it indicates that the action is the default action and not associated with a specific tab.

