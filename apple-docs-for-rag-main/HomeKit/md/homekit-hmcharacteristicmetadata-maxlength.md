

- HomeKit
- HMCharacteristicMetadata
-  maxLength 

Instance Property

# maxLength

The maximum number of UTF-8 characters allowed in a characteristic that uses a string format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var maxLength: NSNumber? { get }
```

## Discussion

This value only applies to characteristics with a string type.

## See Also

### Bounding the value

var validValues: [NSNumber]?

The subset of valid values supported by the characteristic when the format is of type unsigned integer.

var minimumValue: NSNumber?

The minimum value for the characteristic.

var maximumValue: NSNumber?

The maximum value for the characteristic.

var stepValue: NSNumber?

The minimum interval between values for the characteristic.

