

- AppKit
- NSToolbarItem
-  visibilityPriority 

Instance Property

# visibilityPriority

The display priority associated with the toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var visibilityPriority: NSToolbarItem.VisibilityPriority { get set }
```

## Discussion

The default value of this property is standard. Assign a higher priority to give preference to the toolbar item when space is limited.

When a toolbar doesn’t have enough space to fit all of its items, it pushes lower-priority items to the overflow menu first. When two or more items have the same priority, the toolbar removes them one at a time starting from the trailing edge.

## See Also

### Getting the item’s configuration

var isVisible: Bool

A Boolean value that indicates whether the item is currently visible in the toolbar, and not in the overflow menu.

var isBordered: Bool

A Boolean value that indicates whether the toolbar item has a bordered style.

var isNavigational: Bool

A Boolean value that indicates whether the item behaves as a navigation item in the toolbar.

var isEnabled: Bool

A Boolean value that indicates whether the item is enabled.

var allowsDuplicatesInToolbar: Bool

A Boolean value that indicates whether the toolbar item can appear more than once in a toolbar.

Deprecated

struct VisibilityPriority

Constants that indicate which toolbar items to keep in the toolbar when space is limited.

var tag: Int

An integer tag you can use to identify the toolbar item.

