

- AppKit
- NSApplication
-  isAutomaticCustomizeTouchBarMenuItemEnabled 

Instance Property

# isAutomaticCustomizeTouchBarMenuItemEnabled

A Boolean value indicating whether the main menu contains an item for customizing the contents of the Touch Bar.

macOS 10.12.2+

``` source
@MainActor
var isAutomaticCustomizeTouchBarMenuItemEnabled: Bool { get set }
```

## Discussion

When the value of this property is true, AppKit adds a standard item to the app’s View menu that users can select to customize the Touch Bar contents, but only if a Touch Bar is present. If the View menu is unavailable, AppKit adds the item to either the Windows or App menu.

If you prefer to provide a customize menu item, set isAutomaticCustomizeTouchBarMenuItemEnabled to false, and create the menu item with an action of toggleTouchBarCustomizationPalette(_:).

The default value of this property is false.

## See Also

### Accessing the Main Menu

var mainMenu: NSMenu?

The app’s main menu bar.

