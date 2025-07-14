

- AppKit
- NSMenu
-  isTornOff Deprecated

Instance Property

# isTornOff

Indicates whether the menu is offscreen or attached to another menu (or if it’s the main menu).

macOS 10.0–10.11Deprecated

``` source
var isTornOff: Bool { get }
```

## Discussion

This property has a value of false if the menu is offscreen, is attached to another menu, or is the main menu. Otherwise, this property has a value of true.

### Special Considerations

This property has no effect in macOS 10.6 and later.

## See Also

### Managing Submenus

func setSubmenu(NSMenu?, for: NSMenuItem)

Assigns a menu to be a submenu of the menu controlled by a given menu item.

func submenuAction(Any?)

The action method assigned to menu items that open submenus.

var supermenu: NSMenu?

The parent menu that contains the menu as a submenu.

