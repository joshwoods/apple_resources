

- AppKit
- NSStepperCell
-  autorepeat 

Instance Property

# autorepeat

A Boolean value indicating how the receiver responds to mouse events.

macOS

``` source
@MainActor
var autorepeat: Bool { get set }
```

## Discussion

If true, the first mouse down will do one increment (decrement), and, after a delay of 0.5 seconds, will increment (decrement) at a rate of ten times per second. If false, the receiver will do one increment (decrement) on a mouse up. The default is true

## See Also

### Specifying how stepper cell responds

var valueWraps: Bool

A Boolean value indicating whether the receiver wraps around the minimum and maximum values.

