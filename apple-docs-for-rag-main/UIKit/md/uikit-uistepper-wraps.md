

- UIKit
- UIStepper
-  wraps 

Instance Property

# wraps

A Boolean value that determines whether the stepper can wrap its value to the minimum or maximum value when incrementing and decrementing the value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var wraps: Bool { get set }
```

## Discussion

If true, incrementing beyond maximumValue sets value to minimumValue; likewise, decrementing below minimumValue sets value to maximumValue. If false, the stepper doesn’t increment beyond maximumValue nor does it decrement below minimumValue but rather holds at those values.

The default value for this property is false.

## See Also

### Configuring the stepper

var isContinuous: Bool

A Boolean value that determines whether to send value changes during user interaction or after user interaction ends.

var autorepeat: Bool

A Boolean value that determines whether to repeatedly change the stepper’s value as the user presses and holds a stepper button.

var minimumValue: Double

The lowest possible numeric value for the stepper.

var maximumValue: Double

The highest possible numeric value for the stepper.

var stepValue: Double

The step, or increment, value for the stepper.

