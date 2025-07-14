

- AppKit
- NSToolbarItem
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the item is enabled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

If the value of this property is true, the item is enabled. If the autovalidates property is true, changing the value of this property has no effect. Instead, the validation process enables and disables the toolbar item as appropriate.

## See Also

### Related Documentation

var view: NSView?

The custom view you use to draw the toolbar item.

### Getting the item’s configuration

var isVisible: Bool

A Boolean value that indicates whether the item is currently visible in the toolbar, and not in the overflow menu.

var isBordered: Bool

A Boolean value that indicates whether the toolbar item has a bordered style.

var isNavigational: Bool

A Boolean value that indicates whether the item behaves as a navigation item in the toolbar.

var allowsDuplicatesInToolbar: Bool

A Boolean value that indicates whether the toolbar item can appear more than once in a toolbar.

Deprecated

var visibilityPriority: NSToolbarItem.VisibilityPriority

The display priority associated with the toolbar item.

struct VisibilityPriority

Constants that indicate which toolbar items to keep in the toolbar when space is limited.

var tag: Int

An integer tag you can use to identify the toolbar item.

