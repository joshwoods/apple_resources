

- HomeKit
-  HMMutableCharacteristicEvent 

Class

# HMMutableCharacteristicEvent

A mutable event that is evaluated based on the value of a characteristic.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class HMMutableCharacteristicEvent where TriggerValueType : NSCopying
```

## Topics

### Configuring the event

var characteristic: HMCharacteristic

The characteristic associated with the event.

var triggerValue: TriggerValueType?

The value of the characteristic that triggers the event.

## Relationships

### Inherits From

- HMCharacteristicEvent

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

### Characteristics

class HMCharacteristicEvent

An event that is evaluated based on the value of a characteristic.

