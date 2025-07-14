

- Core HID
- HIDElement
- HIDElement.Value
-  init(element:fromBytes:timestamp:) 

Initializer

# init(element:fromBytes:timestamp:)

Creates a value for an HID element.

macOS 15.0+

``` source
init(
    element: HIDElement,
    fromBytes: Data,
    timestamp: SuspendingClock.Instant
)
```

## Parameters 

`element`  

The element associated with this data.

`fromBytes`  

The data as an array of bytes.

`timestamp`  

The time that the value was created.

## Discussion

The created value can be used to send a request to the associated device to update it’s current value for the element using HIDDeviceClient.ProvideElementUpdate.

## See Also

### Create a HID element from a value

init?&lt;FloatingPointType>(element: HIDElement, fromPhysicalValue: FloatingPointType, timestamp: SuspendingClock.Instant)

Creates a HID element value from a physical value.

init?&lt;IntegerType>(element: HIDElement, fromLogicalValueTruncatingIfNeeded: IntegerType, timestamp: SuspendingClock.Instant)

Creates a HID element value from a logical value.

init&lt;IntegerType>(element: HIDElement, fromIntegerTruncatingIfNeeded: IntegerType, timestamp: SuspendingClock.Instant)

Creates an HID element value from an integer.

var element: HIDElement

The HIDElement associated with this value.

