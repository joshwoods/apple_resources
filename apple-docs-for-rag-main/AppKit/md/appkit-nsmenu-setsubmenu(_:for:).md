

- AppKit
- NSMenu
-  setSubmenu(\_:for:) 

Instance Method

# setSubmenu(\_:for:)

Assigns a menu to be a submenu of the menu controlled by a given menu item.

macOS

``` source
func setSubmenu(
    _ menu: NSMenu?,
    for item: NSMenuItem
)
```

## Parameters 

`menu`  

A menu object that is to be a submenu of the menu.

`item`  

A menu item (that is, an object conforming to the NSMenuItem protocol) that controls `aMenu`. The method sets the action of `anItem` to submenuAction(_:).

## See Also

### Managing Submenus

func submenuAction(Any?)

The action method assigned to menu items that open submenus.

var supermenu: NSMenu?

The parent menu that contains the menu as a submenu.

var isTornOff: Bool

Indicates whether the menu is offscreen or attached to another menu (or if it’s the main menu).

Deprecated

