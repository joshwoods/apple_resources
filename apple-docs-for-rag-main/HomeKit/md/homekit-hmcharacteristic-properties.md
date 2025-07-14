

- HomeKit
- HMCharacteristic
-  properties 

Instance Property

# properties

An array of properties that describe the characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var properties: [String] { get }
```

## Discussion

Test a characteristic’s properties array for any of the constants listed in Characteristic Properties to learn something about the corresponding characteristic. For example, you can create a readability Boolean in an extension to the HMCharacteristic class by testing for HMCharacteristicPropertyReadable:

```
extension HMCharacteristic {
    var isReadable: Bool {
        return properties.contains(HMCharacteristicPropertyReadable)
    }
}
```

## See Also

### Reading characteristic properties

Characteristic Properties

The properties that characteristics can have.

