

- AppKit
- NSMenuItem
-  submenu 

Instance Property

# submenu

The submenu of the menu item.

macOS

``` source
var submenu: NSMenu? { get set }
```

## Discussion

The default implementation of the `NSMenuItem` class raises an exception if `aSubmenu` already has a supermenu.

## See Also

### Managing submenus

var hasSubmenu: Bool

A Boolean value that indicates whether the menu item has a submenu.

var parent: NSMenuItem?

The menu item whose submenu contains the receiver.

