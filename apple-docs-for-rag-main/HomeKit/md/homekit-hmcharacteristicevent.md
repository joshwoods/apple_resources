

- HomeKit
-  HMCharacteristicEvent 

Class

# HMCharacteristicEvent

An event that is evaluated based on the value of a characteristic.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMCharacteristicEvent where TriggerValueType : NSCopying
```

## Topics

### Creating a characteristic event

init(characteristic: HMCharacteristic, triggerValue: TriggerValueType?)

Creates a new characteristic event which triggers when the specified characteristic reaches the specified value.

### Inspecting the event

var characteristic: HMCharacteristic

The characteristic associated with the event.

var triggerValue: TriggerValueType?

The value of the characteristic that triggers the event.

### Configuring the event

func updateTriggerValue(TriggerValueType?, completionHandler: ((any Error)?) -> Void)

Changes the trigger value associated with this event.

Deprecated

## Relationships

### Inherits From

- HMEvent

### Inherited By

- HMMutableCharacteristicEvent

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

class HMMutableCharacteristicEvent

A mutable event that is evaluated based on the value of a characteristic.

