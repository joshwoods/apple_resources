

- Core HID
- HIDElement
- HIDElement.Value
-  timestamp 

Instance Property

# timestamp

The time that this data was received by the system.

macOS 15.0+

``` source
var timestamp: SuspendingClock.Instant
```

## Discussion

The data should only be considered valid at this time, it’s possible for the HIDElement to have been updated after this.

## See Also

### Get element data and values

var bytes: Data

The data as an array of bytes.

func integerValue&lt;IntegerType>(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType

The raw value of the data cast as an integer type, with no transformations applied.

func logicalValue&lt;IntegerType>(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType?

The raw value of the data cast as an integer type and bound by the HIDElement’s logical minimum and logical maximum values.

func physicalValue&lt;IntegerType, FloatingType>(fromTypeTruncatingIfNeeded: IntegerType.Type, as: FloatingType.Type) -> FloatingType?

The logical value of the data, shifted and scaled by the HIDElement’s physical minimum, physical maximum and exponent.

