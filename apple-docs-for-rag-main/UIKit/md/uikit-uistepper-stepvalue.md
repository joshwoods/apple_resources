

- UIKit
- UIStepper
-  stepValue 

Instance Property

# stepValue

The step, or increment, value for the stepper.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var stepValue: Double { get set }
```

## Discussion

Must be numerically greater than `0`. If you attempt to set this property’s value to `0` or to a negative number, the system raises an invalidArgumentException exception.

The default value for this property is `1`.

## See Also

### Configuring the stepper

var isContinuous: Bool

A Boolean value that determines whether to send value changes during user interaction or after user interaction ends.

var autorepeat: Bool

A Boolean value that determines whether to repeatedly change the stepper’s value as the user presses and holds a stepper button.

var wraps: Bool

A Boolean value that determines whether the stepper can wrap its value to the minimum or maximum value when incrementing and decrementing the value.

var minimumValue: Double

The lowest possible numeric value for the stepper.

var maximumValue: Double

The highest possible numeric value for the stepper.

