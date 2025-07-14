

- AppKit
- NSStatusItem
-  behavior 

Instance Property

# behavior

The set of allowed behaviors for the status item.

macOS 10.12+

``` source
var behavior: NSStatusItem.Behavior { get set }
```

## Discussion

By default, this property includes no behavior options. See NSStatusItem.Behavior for a list of available behavior options and their effects.

## See Also

### Managing the Status Item’s Behavior

struct Behavior

A set of optional status item behaviors.

var button: NSStatusBarButton?

The button displayed in the status bar.

var menu: NSMenu?

The pull-down menu displayed when the user clicks the status item.

