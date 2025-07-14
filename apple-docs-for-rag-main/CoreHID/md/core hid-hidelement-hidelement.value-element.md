

- Core HID
- HIDElement
- HIDElement.Value
-  element 

Instance Property

# element

The HIDElement associated with this value.

macOS 15.0+

``` source
var element: HIDElement
```

## See Also

### Create a HID element from a value

init(element: HIDElement, fromBytes: Data, timestamp: SuspendingClock.Instant)

Creates a value for an HID element.

init?&lt;FloatingPointType>(element: HIDElement, fromPhysicalValue: FloatingPointType, timestamp: SuspendingClock.Instant)

Creates a HID element value from a physical value.

init?&lt;IntegerType>(element: HIDElement, fromLogicalValueTruncatingIfNeeded: IntegerType, timestamp: SuspendingClock.Instant)

Creates a HID element value from a logical value.

init&lt;IntegerType>(element: HIDElement, fromIntegerTruncatingIfNeeded: IntegerType, timestamp: SuspendingClock.Instant)

Creates an HID element value from an integer.

