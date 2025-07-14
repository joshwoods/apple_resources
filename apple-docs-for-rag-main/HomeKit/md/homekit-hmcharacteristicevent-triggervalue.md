

- HomeKit
- HMCharacteristicEvent
-  triggerValue 

Instance Property

# triggerValue

The value of the characteristic that triggers the event.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var triggerValue: TriggerValueType? { get }
```

## Discussion

A value of `nil` corresponds to any change in the value of the characteristic.

## See Also

### Inspecting the event

var characteristic: HMCharacteristic

The characteristic associated with the event.

