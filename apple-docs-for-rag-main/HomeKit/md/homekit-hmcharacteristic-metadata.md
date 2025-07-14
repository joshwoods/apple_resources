

- HomeKit
- HMCharacteristic
-  metadata 

Instance Property

# metadata

Metadata about the units and other properties of the characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var metadata: HMCharacteristicMetadata? { get }
```

## Discussion

You can typically infer a lot about a characteristic’s value from its characteristicType, like if the value is a string, a number, or in some other format; what the units are; and what range of values to expect. To obtain this information explicitly, inspect the characteristic’s metadata, represented by an instance of the HMCharacteristicMetadata class.

## See Also

### Managing characteristic presentation

class HMCharacteristicMetadata

Metadata that describes a characteristic’s value and that may be useful for presentation purposes.

