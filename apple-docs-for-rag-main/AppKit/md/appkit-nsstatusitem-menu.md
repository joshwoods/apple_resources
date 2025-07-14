

- AppKit
- NSStatusItem
-  menu 

Instance Property

# menu

The pull-down menu displayed when the user clicks the status item.

macOS

``` source
var menu: NSMenu? { get set }
```

## Discussion

When non-`nil`, the status item’s single click action behavior is not used. Setting the value of this property to `nil` removes the menu.

## See Also

### Managing the Status Item’s Behavior

var behavior: NSStatusItem.Behavior

The set of allowed behaviors for the status item.

struct Behavior

A set of optional status item behaviors.

var button: NSStatusBarButton?

The button displayed in the status bar.

