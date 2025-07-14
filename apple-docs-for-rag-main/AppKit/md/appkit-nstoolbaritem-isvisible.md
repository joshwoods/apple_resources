

- AppKit
- NSToolbarItem
-  isVisible 

Instance Property

# isVisible

A Boolean value that indicates whether the item is currently visible in the toolbar, and not in the overflow menu.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+

``` source
@MainActor
var isVisible: Bool { get }
```

## Discussion

The value of this property is true when the item is visible in the toolbar, and false when it isn’t in the toolbar or is present in the toolbar’s overflow menu. This property is key-value observing (KVO) compliant.

## See Also

### Getting the item’s configuration

var isBordered: Bool

A Boolean value that indicates whether the toolbar item has a bordered style.

var isNavigational: Bool

A Boolean value that indicates whether the item behaves as a navigation item in the toolbar.

var isEnabled: Bool

A Boolean value that indicates whether the item is enabled.

var allowsDuplicatesInToolbar: Bool

A Boolean value that indicates whether the toolbar item can appear more than once in a toolbar.

Deprecated

var visibilityPriority: NSToolbarItem.VisibilityPriority

The display priority associated with the toolbar item.

struct VisibilityPriority

Constants that indicate which toolbar items to keep in the toolbar when space is limited.

var tag: Int

An integer tag you can use to identify the toolbar item.

