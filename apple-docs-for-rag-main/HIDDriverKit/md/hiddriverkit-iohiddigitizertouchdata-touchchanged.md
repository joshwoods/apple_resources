

- HIDDriverKit
- IOHIDDigitizerTouchData
-  touchChanged 

Instance Property

# touchChanged

A single-bit Boolean that indicates whether the touch variable changed since the last event was dispatched.

DriverKitmacOS

``` source
uint32_t touchChanged;
```

## Discussion

For example, this property is `1` if the value in the touch field changed from `0` to `1` since the last event.

## See Also

### Getting the Touch Data

identifier

A unique contact identifier.

x

An x-coordinate value in the range `0.0` to `1.0`.

y

A y-coordinate value in the range `0.0` to `1.0`.

inRange

A single-bit Boolean that indicates whether the finger is in range.

touch

A single-bit Boolean that indicates whether the finger is in contact with the surface of the digitizer.

touchValid

A single-bit Boolean that indicates whether the touch contact was intended.

positionChanged

A single-bit Boolean that indicates whether the x or y position changed since the last event was dispatched.

rangeChanged

A single-bit Boolean that indicates whether the range variable changed since the last event was dispatched.

