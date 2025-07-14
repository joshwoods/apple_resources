

- HomeKit
-  HMCharacteristicThresholdRangeEvent 

Class

# HMCharacteristicThresholdRangeEvent

An event that triggers when the value of a characteristic is within a specified range.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class HMCharacteristicThresholdRangeEvent
```

## Topics

### Creating a characteristic threshold range event

init(characteristic: HMCharacteristic, thresholdRange: HMNumberRange)

Creates a characteristic threshold range event for the specified characteristic and number range.

### Inspecting a characteristic threshold event

var characteristic: HMCharacteristic

The characteristic associated with the event.

var thresholdRange: HMNumberRange

The range of the characteristic value that triggers the event.

## Relationships

### Inherits From

- HMEvent

### Inherited By

- HMMutableCharacteristicThresholdRangeEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- Sendable

## See Also

### Characteristic ranges

class HMNumberRange

A set of numbers used to specify conditions for characteristic range threshold events.

class HMMutableCharacteristicThresholdRangeEvent

A mutable event that triggers when the value of a characteristic is within a specified range.

