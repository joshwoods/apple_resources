

- HomeKit
-  HMNumberRange 

Class

# HMNumberRange

A set of numbers used to specify conditions for characteristic range threshold events.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class HMNumberRange
```

## Topics

### Creating a number range

convenience init(minValue: NSNumber, maxValue: NSNumber)

Creates a new number range.

convenience init(minValue: NSNumber)

Creates an one-sided number range with a minimum value.

convenience init(maxValue: NSNumber)

Creates a one-sided number range with a maximum value.

### Inspecting a number range

var minValue: NSNumber?

The minimum value of the range.

var maxValue: NSNumber?

The maximum value of the range.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Characteristic ranges

class HMCharacteristicThresholdRangeEvent

An event that triggers when the value of a characteristic is within a specified range.

class HMMutableCharacteristicThresholdRangeEvent

A mutable event that triggers when the value of a characteristic is within a specified range.

