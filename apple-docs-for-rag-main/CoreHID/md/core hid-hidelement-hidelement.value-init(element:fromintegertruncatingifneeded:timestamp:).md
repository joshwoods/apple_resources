

- Core HID
- HIDElement
- HIDElement.Value
-  init(element:fromIntegerTruncatingIfNeeded:timestamp:) 

Initializer

# init(element:fromIntegerTruncatingIfNeeded:timestamp:)

Creates an HID element value from an integer.

macOS 15.0+

``` source
init(
    element: HIDElement,
    fromIntegerTruncatingIfNeeded: IntegerType,
    timestamp: SuspendingClock.Instant
) where IntegerType : FixedWidthInteger
```

## Parameters 

`element`  

The element associated with this value.

`fromIntegerTruncatingIfNeeded`  

An integer to use for the value’s bytes, truncating or extending the bytes as necessary.

`timestamp`  

The time that the value was created.

## Discussion

The logical and physical values are calculated, but don’t need to be valid.

## See Also

### Create a HID element from a value

init(element: HIDElement, fromBytes: Data, timestamp: SuspendingClock.Instant)

Creates a value for an HID element.

init?&lt;FloatingPointType>(element: HIDElement, fromPhysicalValue: FloatingPointType, timestamp: SuspendingClock.Instant)

Creates a HID element value from a physical value.

init?&lt;IntegerType>(element: HIDElement, fromLogicalValueTruncatingIfNeeded: IntegerType, timestamp: SuspendingClock.Instant)

Creates a HID element value from a logical value.

var element: HIDElement

The HIDElement associated with this value.

