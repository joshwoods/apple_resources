

- AppKit
- NSToolbarItem
-  isNavigational 

Instance Property

# isNavigational

A Boolean value that indicates whether the item behaves as a navigation item in the toolbar.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
@MainActor
var isNavigational: Bool { get set }
```

## Discussion

Mark a toolbar item as navigation if you use it to navigate around your content. When you set this property to true, the system can position navigation items outside of the normal list of items in the toolbar. For example, the back and forward buttons in Finder windows are navigational, and the system positions them at the leading edge of the window’s title area. Specify the initial order of the items using the toolbarDefaultItemIdentifiers(_:) method of the toolbar delegate object.

## See Also

### Getting the item’s configuration

var isVisible: Bool

A Boolean value that indicates whether the item is currently visible in the toolbar, and not in the overflow menu.

var isBordered: Bool

A Boolean value that indicates whether the toolbar item has a bordered style.

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

