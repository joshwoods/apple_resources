

- AppKit
- NSMenu
-  autoenablesItems 

Instance Property

# autoenablesItems

Indicates whether the menu automatically enables and disables its menu items.

macOS

``` source
var autoenablesItems: Bool { get set }
```

## Discussion

This property contains a Boolean value, indicating whether the menu automatically enables and disables its menu items. If set to true, menu items of the menu are automatically enabled and disabled according to rules computed by the NSMenuValidation informal protocol. By default, `NSMenu` objects autoenable their menu items.

## See Also

### Enabling and Disabling Menu Items

func update()

Enables or disables the menu items of the menu based on the NSMenuValidation informal protocol and sizes the menu to fit its current menu items if necessary.

