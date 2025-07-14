

- AppKit
- NSSwitch
-  state 

Instance Property

# state

The current position of the switch.

macOS 10.15+

``` source
@MainActor
var state: NSControl.StateValue { get set }
```

## Discussion

The values off and on indicate that the switch is in the off or on position. The switch treats any value other than off as on.

Setting this property through the animator() proxy animates the switch to the new value.

