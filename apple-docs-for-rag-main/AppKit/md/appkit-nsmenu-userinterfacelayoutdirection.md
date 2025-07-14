

- AppKit
- NSMenu
-  userInterfaceLayoutDirection 

Instance Property

# userInterfaceLayoutDirection

Configures the layout direction of menu items in the menu.

macOS 10.11+

``` source
var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection { get set }
```

## Discussion

This property configures the layout direction (a value of type NSUserInterfaceLayoutDirection) of menu items in the menu. If no layout direction is explicitly set for a menu, then the menu defaults to the layout direction specified for the application object. See userInterfaceLayoutDirection in NSApplication.

## See Also

### Related Documentation

enum NSUserInterfaceLayoutDirection

Specifies the directional flow of the user interface.

