

- AppKit
- NSComboButton
-  menu 

Instance Property

# menu

The menu that contains the button’s alternate actions.

macOS 13.0+

``` source
@MainActor
var menu: NSMenu { get set }
```

## Discussion

The combo button executes the menu item’s action when someone selects that item, so make sure to configure the targets and actions for each menu item in your menu.

An NSComboButton doesn’t support the addition of a contextual menu.

