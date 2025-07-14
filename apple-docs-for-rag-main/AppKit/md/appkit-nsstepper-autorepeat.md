

- AppKit
- NSStepper
-  autorepeat 

Instance Property

# autorepeat

A Boolean value that indicates how the stepper responds to mouse events.

macOS

``` source
@MainActor
var autorepeat: Bool { get set }
```

## Discussion

true if the first mouse down does one increment (or decrement) and, after a delay of 0.5 seconds, increments (or decrements) at a rate of ten times per second. false if the receiver does one increment (decrement) on a mouse up. The default is true.

## See Also

### Specifying how the stepper responds

var valueWraps: Bool

A Boolean value that indicates whether the stepper wraps around the minimum and maximum values.

