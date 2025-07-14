

- Core HID
- HIDElement
- HIDElement.Value
-  physicalValue(fromTypeTruncatingIfNeeded:as:) 

Instance Method

# physicalValue(fromTypeTruncatingIfNeeded:as:)

The logical value of the data, shifted and scaled by the HIDElement’s physical minimum, physical maximum and exponent.

macOS 15.0+

``` source
func physicalValue(
    fromTypeTruncatingIfNeeded: IntegerType.Type,
    as: FloatingType.Type
) -> FloatingType? where IntegerType : FixedWidthInteger, FloatingType : BinaryFloatingPoint
```

## Parameters 

`fromTypeTruncatingIfNeeded`  

The type to cast the underlying bytes to before bounding, shifting and scaling; truncating or extending the bytes as necessary.

`as`  

The type to cast the calculated floating point result to before returning.

## Return Value

The calculated value cast as the requested type, or nil if out of bounds.

## Discussion

The logicalValue(asTypeTruncatingIfNeeded:) is first retrieved with the specified type. If the logical value is undefined, such as when the raw value is out of bounds, the physical value is also undefined.

More information and example calculations for physical values can be found in the HID specification: See the HID specification for more details: https://www.usb.org/hid.

## See Also

### Get element data and values

var bytes: Data

The data as an array of bytes.

func integerValue&lt;IntegerType>(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType

The raw value of the data cast as an integer type, with no transformations applied.

func logicalValue&lt;IntegerType>(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType?

The raw value of the data cast as an integer type and bound by the HIDElement’s logical minimum and logical maximum values.

var timestamp: SuspendingClock.Instant

The time that this data was received by the system.

