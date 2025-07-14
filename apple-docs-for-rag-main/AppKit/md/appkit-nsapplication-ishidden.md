

- AppKit
- NSApplication
-  isHidden 

Instance Property

# isHidden

A Boolean value indicating whether the app is hidden.

macOS

``` source
@MainActor
var isHidden: Bool { get }
```

## Discussion

The value of this property is true if the app is hidden or false if it is not.

## See Also

### Hiding Windows

func hide(Any?)

Hides all the receiver’s windows, and the next app in line is activated.

func unhide(Any?)

Restores hidden windows to the screen and makes the receiver active.

func unhideWithoutActivation()

Restores hidden windows without activating their owner (the receiver).

