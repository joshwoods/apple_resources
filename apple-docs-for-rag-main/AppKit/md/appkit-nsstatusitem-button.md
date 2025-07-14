

- AppKit
- NSStatusItem
-  button 

Instance Property

# button

The button displayed in the status bar.

macOS 10.10+

``` source
var button: NSStatusBarButton? { get }
```

## Discussion

The status item automatically creates this button by default. Use this property to customize the appearance and behavior of the button, such as its image, target, action, toolTip, and so on.

## See Also

### Managing the Status Item’s Behavior

var behavior: NSStatusItem.Behavior

The set of allowed behaviors for the status item.

struct Behavior

A set of optional status item behaviors.

var menu: NSMenu?

The pull-down menu displayed when the user clicks the status item.

