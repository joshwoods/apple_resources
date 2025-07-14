

- AppKit
-  NSStepperCell 

Class

# NSStepperCell

An `NSStepperCell` object controls the appearance and behavior of an NSStepper object.

macOS

``` source
@MainActor
class NSStepperCell
```

## Topics

### Specifying value range

var maxValue: Double

The maximum value for the receiver.

var minValue: Double

The minimum value for the receiver.

var increment: Double

The amount by which the receiver will change per increment or decrement.

### Specifying how stepper cell responds

var autorepeat: Bool

A Boolean value indicating how the receiver responds to mouse events.

var valueWraps: Bool

A Boolean value indicating whether the receiver wraps around the minimum and maximum values.

## Relationships

### Inherits From

- NSActionCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

