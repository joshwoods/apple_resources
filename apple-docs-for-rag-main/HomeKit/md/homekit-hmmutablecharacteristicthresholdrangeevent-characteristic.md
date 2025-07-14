

- HomeKit
- HMMutableCharacteristicThresholdRangeEvent
-  characteristic 

Instance Property

# characteristic

The characteristic associated with the event.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var characteristic: HMCharacteristic { get set }
```

## Discussion

Use this property to change the event’s characteristic.

The characteristic must support notification.

## See Also

### Configuring a characteristic threshold event

var thresholdRange: HMNumberRange

The range of the characteristic value that triggers the event.

