

- Core HID
- HIDElement
- HIDElement.Value
-  integerValue(asTypeTruncatingIfNeeded:) 

Instance Method

# integerValue(asTypeTruncatingIfNeeded:)

The raw value of the data cast as an integer type, with no transformations applied.

macOS 15.0+

``` source
func integerValue(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType where IntegerType : FixedWidthInteger
```

## Parameters 

`asTypeTruncatingIfNeeded`  

The type to which to cast the underlying bytes, truncating or extending the bytes as necessary.

## Return Value

The data cast as the requested type.

## Mentioned in 

Communicating with human interface devices

## See Also

### Get element data and values

var bytes: Data

The data as an array of bytes.

func logicalValue&lt;IntegerType>(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType?

The raw value of the data cast as an integer type and bound by the HIDElement’s logical minimum and logical maximum values.

func physicalValue&lt;IntegerType, FloatingType>(fromTypeTruncatingIfNeeded: IntegerType.Type, as: FloatingType.Type) -> FloatingType?

The logical value of the data, shifted and scaled by the HIDElement’s physical minimum, physical maximum and exponent.

var timestamp: SuspendingClock.Instant

The time that this data was received by the system.

