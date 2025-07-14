

- UIKit
- UIStepper
-  autorepeat 

Instance Property

# autorepeat

A Boolean value that determines whether to repeatedly change the stepper’s value as the user presses and holds a stepper button.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var autorepeat: Bool { get set }
```

## Discussion

If true, the user pressing and holding on the stepper repeatedly alters value.

The default value for this property is true.

## See Also

### Configuring the stepper

var isContinuous: Bool

A Boolean value that determines whether to send value changes during user interaction or after user interaction ends.

var wraps: Bool

A Boolean value that determines whether the stepper can wrap its value to the minimum or maximum value when incrementing and decrementing the value.

var minimumValue: Double

The lowest possible numeric value for the stepper.

var maximumValue: Double

The highest possible numeric value for the stepper.

var stepValue: Double

The step, or increment, value for the stepper.

