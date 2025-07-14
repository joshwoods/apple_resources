

- HomeKit
- HMCharacteristic
-  characteristicType 

Instance Property

# characteristicType

The type of the characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var characteristicType: String { get }
```

## Discussion

A characteristic’s characteristicType is a string constant that tells you what the characteristic’s value represents. For example, if you detect a characteristic type of HMCharacteristicTypeCurrentTemperature, then you know that the corresponding value is a measure of the current temperature.

```
if characteristic.characteristicType == HMCharacteristicTypeCurrentTemperature,
    let temperatureValue = (characteristic.value as? NSNumber)?.floatValue {

    let temperature = String(format: "%.1f", temperatureValue)
    print("The current temperature is \(temperature) °C")
}
```

From the type, you can typically infer the value’s format. The value for the current temperature is always a floating point number measured in degrees Celsius, as shown in the code snippet above. You can also use the characteristic’s metadata to get explicit and detailed guidance on how to format the value.

See Characteristic types for a list of standard types.

## See Also

### Determining what a characteristic controls

Characteristic types

The characteristic types supported by HomeKit-based accessories.

