

- UIKit
- UIStepper
-  minimumValue 

Instance Property

# minimumValue

The lowest possible numeric value for the stepper.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var minimumValue: Double { get set }
```

## Discussion

Must be numerically less than maximumValue. If you attempt to set a value equal to or greater than maximumValue, the system raises an invalidArgumentException exception.

The default value for this property is `0`.

## See Also

### Configuring the stepper

var isContinuous: Bool

A Boolean value that determines whether to send value changes during user interaction or after user interaction ends.

var autorepeat: Bool

A Boolean value that determines whether to repeatedly change the stepper’s value as the user presses and holds a stepper button.

var wraps: Bool

A Boolean value that determines whether the stepper can wrap its value to the minimum or maximum value when incrementing and decrementing the value.

var maximumValue: Double

The highest possible numeric value for the stepper.

var stepValue: Double

The step, or increment, value for the stepper.

