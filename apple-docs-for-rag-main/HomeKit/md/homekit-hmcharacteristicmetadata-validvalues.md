

- HomeKit
- HMCharacteristicMetadata
-  validValues 

Instance Property

# validValues

The subset of valid values supported by the characteristic when the format is of type unsigned integer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var validValues: [NSNumber]? { get }
```

## See Also

### Bounding the value

var minimumValue: NSNumber?

The minimum value for the characteristic.

var maximumValue: NSNumber?

The maximum value for the characteristic.

var stepValue: NSNumber?

The minimum interval between values for the characteristic.

var maxLength: NSNumber?

The maximum number of UTF-8 characters allowed in a characteristic that uses a string format.

