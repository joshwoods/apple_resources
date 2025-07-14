

- UIKit
- UIStepper
-  value 

Instance Property

# value

The numeric value of the stepper.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var value: Double { get set }
```

## Discussion

When the value changes, the stepper sends the valueChanged flag to its target (see addTarget(_:action:for:)). Refer to the description of the isContinuous property for information about whether value change events are sent continuously or when user interaction ends.

The default value for this property is `0`. This property is clamped at its lower extreme to minimumValue and is clamped at its upper extreme to maximumValue.

