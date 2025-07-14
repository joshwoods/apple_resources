

- UIKit
- UIStepper
-  isContinuous 

Instance Property

# isContinuous

A Boolean value that determines whether to send value changes during user interaction or after user interaction ends.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isContinuous: Bool { get set }
```

## Discussion

If true, the stepper sends value change events immediately as the value changes during user interaction. If false, the stepper sends a value change event after user interaction ends.

The default value for this property is true.

## See Also

### Configuring the stepper

var autorepeat: Bool

A Boolean value that determines whether to repeatedly change the stepper’s value as the user presses and holds a stepper button.

var wraps: Bool

A Boolean value that determines whether the stepper can wrap its value to the minimum or maximum value when incrementing and decrementing the value.

var minimumValue: Double

The lowest possible numeric value for the stepper.

var maximumValue: Double

The highest possible numeric value for the stepper.

var stepValue: Double

The step, or increment, value for the stepper.

