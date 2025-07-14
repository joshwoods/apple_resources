

- AppKit
- NSToolbarItem
-  allowsDuplicatesInToolbar Deprecated

Instance Property

# allowsDuplicatesInToolbar

A Boolean value that indicates whether the toolbar item can appear more than once in a toolbar.

macOS 10.0–15.0Deprecated

``` source
@MainActor
var allowsDuplicatesInToolbar: Bool { get }
```

Deprecated

Duplicates are no longer supported.

## Discussion

If the value in this property is true, the toolbar allows someone to drag more than one copy of the toolbar item from the customization palette. If the value of this property is false, the toolbar prevents someone from dragging more than one copy of the item from the customization palette.

By default, if an item with the same identifier is already in the toolbar, dragging it in again will effectively move it to the new position.

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

var visibilityPriority: NSToolbarItem.VisibilityPriority

The display priority associated with the toolbar item.

struct VisibilityPriority

Constants that indicate which toolbar items to keep in the toolbar when space is limited.

var tag: Int

An integer tag you can use to identify the toolbar item.

