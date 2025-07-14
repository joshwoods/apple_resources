

- Core HID
- HIDElement
- HIDElement.Value
-  logicalValue(asTypeTruncatingIfNeeded:) 

Instance Method

# logicalValue(asTypeTruncatingIfNeeded:)

The raw value of the data cast as an integer type and bound by the HIDElement’s logical minimum and logical maximum values.

macOS 15.0+

``` source
func logicalValue(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType? where IntegerType : FixedWidthInteger
```

## Parameters 

`asTypeTruncatingIfNeeded`  

The type to which to cast the underlying bytes before applying bounds, truncating or extending the bytes as necessary.

## Return Value

The data cast as the requested type, or nil if out of bounds.

## Discussion

If the raw value is out of bounds, this returns `nil`. For example, if the logical minimum and logical maximum are specified as `1` and `127` respectively, and the raw value is `0`, the logical value is undefined.

## See Also

### Get element data and values

var bytes: Data

The data as an array of bytes.

func integerValue&lt;IntegerType>(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType

The raw value of the data cast as an integer type, with no transformations applied.

func physicalValue&lt;IntegerType, FloatingType>(fromTypeTruncatingIfNeeded: IntegerType.Type, as: FloatingType.Type) -> FloatingType?

The logical value of the data, shifted and scaled by the HIDElement’s physical minimum, physical maximum and exponent.

var timestamp: SuspendingClock.Instant

The time that this data was received by the system.

