

- HomeKit
- HMCharacteristicMetadata
-  format 

Instance Property

# format

The format of the values for the characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var format: String? { get }
```

## Discussion

The format property tells you what kind of data the characteristic’s value contains. For example, you can extend the HMCharacteristic class with a computed property that reports whether a given characteristic is a floating point number:

```
extension HMCharacteristic {
    var isFloat: Bool {
        return metadata?.format == HMCharacteristicMetadataFormatFloat
    }
}
```

See Characteristic Data Formats for the list of possible formats.

## See Also

### Formatting the value

Characteristic Data Formats

Constants for identifying the data format of characteristic values.

