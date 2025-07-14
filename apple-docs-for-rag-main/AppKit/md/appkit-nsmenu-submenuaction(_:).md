

- AppKit
- NSMenu
-  submenuAction(\_:) 

Instance Method

# submenuAction(\_:)

The action method assigned to menu items that open submenus.

macOS

``` source
func submenuAction(_ sender: Any?)
```

## Discussion

You may override this method to implement different behavior. Never invoke this method directly.

## See Also

### Managing Submenus

func setSubmenu(NSMenu?, for: NSMenuItem)

Assigns a menu to be a submenu of the menu controlled by a given menu item.

var supermenu: NSMenu?

The parent menu that contains the menu as a submenu.

var isTornOff: Bool

Indicates whether the menu is offscreen or attached to another menu (or if it’s the main menu).

Deprecated

