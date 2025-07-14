

- UIKit
- UIStepper
-  maximumValue 

Instance Property

# maximumValue

The highest possible numeric value for the stepper.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var maximumValue: Double { get set }
```

## Discussion

Must be numerically greater than minimumValue. If you attempt to set a value equal to or lower than minimumValue, the system raises an invalidArgumentException exception.

The default value of this property is `100`.

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

var stepValue: Double

The step, or increment, value for the stepper.

