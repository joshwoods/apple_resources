

- AppKit
- NSToolbarItem
-  isBordered 

Instance Property

# isBordered

A Boolean value that indicates whether the toolbar item has a bordered style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
var isBordered: Bool { get set }
```

## Discussion

If your toolbar item displays a custom view, modifying this property applies the image to the view’s isBordered property, if one exists. The default value of this property is false.

Note

In macOS 12 and earlier, NSToolbarItem doesn’t support custom views in Mac apps built with Mac Catalyst.

## See Also

### Getting the item’s configuration

var isVisible: Bool

A Boolean value that indicates whether the item is currently visible in the toolbar, and not in the overflow menu.

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

