

- AppKit
- NSStepper
-  valueWraps 

Instance Property

# valueWraps

A Boolean value that indicates whether the stepper wraps around the minimum and maximum values.

macOS

``` source
@MainActor
var valueWraps: Bool { get set }
```

## Discussion

true if, when incrementing or decrementing, the value wraps around to the minimum or maximum. false if the value stays pinned at the minimum or maximum. The default is true.

## See Also

### Specifying how the stepper responds

var autorepeat: Bool

A Boolean value that indicates how the stepper responds to mouse events.

