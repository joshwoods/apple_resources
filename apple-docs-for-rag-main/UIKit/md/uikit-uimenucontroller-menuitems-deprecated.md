

- UIKit
- UIMenuController
-  menuItems Deprecated

Instance Property

# menuItems

The custom menu items for the editing menu.

iOS 3.2–16.0DeprecatediPadOS 3.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var menuItems: [UIMenuItem]? { get set }
```

## Discussion

The default value is `nil` (no custom menu items). Each menu item is an instance of the UIMenuItem class. You may create your own menu items, each with its own title and action selector, and add them to the editing menu through this property. Custom items appear in the menu after any system menu items.

