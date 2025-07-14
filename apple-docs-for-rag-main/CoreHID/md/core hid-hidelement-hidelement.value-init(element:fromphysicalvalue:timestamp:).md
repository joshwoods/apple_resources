

- Core HID
- HIDElement
- HIDElement.Value
-  init(element:fromPhysicalValue:timestamp:) 

Initializer

# init(element:fromPhysicalValue:timestamp:)

Creates a HID element value from a physical value.

macOS 15.0+

``` source
init?(
    element: HIDElement,
    fromPhysicalValue: FloatingPointType,
    timestamp: SuspendingClock.Instant
) where FloatingPointType : BinaryFloatingPoint
```

## Parameters 

`element`  

The element associated with this value.

`timestamp`  

The time that the value was created.

## Discussion

The raw value and physical value are calculated; both must be valid.

## See Also

### Create a HID element from a value

init(element: HIDElement, fromBytes: Data, timestamp: SuspendingClock.Instant)

Creates a value for an HID element.

init?&lt;IntegerType>(element: HIDElement, fromLogicalValueTruncatingIfNeeded: IntegerType, timestamp: SuspendingClock.Instant)

Creates a HID element value from a logical value.

init&lt;IntegerType>(element: HIDElement, fromIntegerTruncatingIfNeeded: IntegerType, timestamp: SuspendingClock.Instant)

Creates an HID element value from an integer.

var element: HIDElement

The HIDElement associated with this value.

