

- HomeKit
- HMMutableCharacteristicThresholdRangeEvent
-  thresholdRange 

Instance Property

# thresholdRange

The range of the characteristic value that triggers the event.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@NSCopying
var thresholdRange: HMNumberRange { get set }
```

## Discussion

Use this property to adjust the range of characteristic values that trigger the event.

## See Also

### Configuring a characteristic threshold event

var characteristic: HMCharacteristic

The characteristic associated with the event.

