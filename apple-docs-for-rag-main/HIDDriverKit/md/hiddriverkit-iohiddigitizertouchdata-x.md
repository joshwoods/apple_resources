

- HIDDriverKit
- IOHIDDigitizerTouchData
-  x 

Instance Property

# x

An x-coordinate value in the range `0.0` to `1.0`.

DriverKitmacOS

``` source
IOFixed x;
```

## See Also

### Getting the Touch Data

identifier

A unique contact identifier.

y

A y-coordinate value in the range `0.0` to `1.0`.

inRange

A single-bit Boolean that indicates whether the finger is in range.

touch

A single-bit Boolean that indicates whether the finger is in contact with the surface of the digitizer.

touchValid

A single-bit Boolean that indicates whether the touch contact was intended.

touchChanged

A single-bit Boolean that indicates whether the touch variable changed since the last event was dispatched.

positionChanged

A single-bit Boolean that indicates whether the x or y position changed since the last event was dispatched.

rangeChanged

A single-bit Boolean that indicates whether the range variable changed since the last event was dispatched.

