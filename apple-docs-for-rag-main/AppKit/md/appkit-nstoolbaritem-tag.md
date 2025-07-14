

- AppKit
- NSToolbarItem
-  tag 

Instance Property

# tag

An integer tag you can use to identify the toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var tag: Int { get set }
```

## Discussion

The toolbar doesn’t use this value. You can use it for your own custom purposes.

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

var visibilityPriority: NSToolbarItem.VisibilityPriority

The display priority associated with the toolbar item.

struct VisibilityPriority

Constants that indicate which toolbar items to keep in the toolbar when space is limited.

