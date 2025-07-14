

- Core HID
- HIDElement
- HIDElement.Value
-  bytes 

Instance Property

# bytes

The data as an array of bytes.

macOS 15.0+

``` source
var bytes: Data
```

## Mentioned in 

Communicating with human interface devices

## Discussion

The size of the data must be the elements reportSize, rounded up to the next byte.

## See Also

### Get element data and values

func integerValue&lt;IntegerType>(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType

The raw value of the data cast as an integer type, with no transformations applied.

func logicalValue&lt;IntegerType>(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType?

The raw value of the data cast as an integer type and bound by the HIDElement’s logical minimum and logical maximum values.

func physicalValue&lt;IntegerType, FloatingType>(fromTypeTruncatingIfNeeded: IntegerType.Type, as: FloatingType.Type) -> FloatingType?

The logical value of the data, shifted and scaled by the HIDElement’s physical minimum, physical maximum and exponent.

var timestamp: SuspendingClock.Instant

The time that this data was received by the system.

