

- AppKit
- NSToolbarItem
-  itemMenuFormRepresentation 

Instance Property

# itemMenuFormRepresentation

The menu item to use for the toolbar item is in the overflow menu in a Mac app built with Mac Catalyst.

Mac Catalyst 13.0+

``` source
@NSCopying @MainActor
var itemMenuFormRepresentation: UIMenuElement? { get set }
```

## Discussion

The toolbar provides an initial default menu form representation that uses the toolbar item’s label as the menu item’s title. You can customize this menu item by changing the title or adding a submenu. When the toolbar is in text only mode, this menu item provides the text for the toolbar item. If the menu item in this property has a submenu and is visbile, clicking the toolbar item displays that submenu. If the toolbar item isn’t visible because it’s in the overflow menu, the menu item and submenu appear there.

For a discussion on menu forms, see Setting a Toolbar Item’s Representation.

## See Also

### Configuring the item’s menu

var menuFormRepresentation: NSMenuItem?

The menu item to use when the toolbar item is in the overflow menu.

