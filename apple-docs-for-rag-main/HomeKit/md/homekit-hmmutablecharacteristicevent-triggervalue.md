

- HomeKit
- HMMutableCharacteristicEvent
-  triggerValue 

Instance Property

# triggerValue

The value of the characteristic that triggers the event.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@NSCopying
var triggerValue: TriggerValueType? { get set }
```

## Discussion

Use this property to adjust the value that triggers the event.

Set this property to `nil` to trigger the event whenever the value of the characteristic changes.

## See Also

### Configuring the event

var characteristic: HMCharacteristic

The characteristic associated with the event.

