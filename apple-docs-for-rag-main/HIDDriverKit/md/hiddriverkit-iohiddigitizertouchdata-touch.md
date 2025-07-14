

- HIDDriverKit
- IOHIDDigitizerTouchData
-  touch 

Instance Property

# touch

A single-bit Boolean that indicates whether the finger is in contact with the surface of the digitizer.

DriverKitmacOS

``` source
uint32_t touch;
```

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

touchValid

A single-bit Boolean that indicates whether the touch contact was intended.

touchChanged

A single-bit Boolean that indicates whether the touch variable changed since the last event was dispatched.

positionChanged

A single-bit Boolean that indicates whether the x or y position changed since the last event was dispatched.

rangeChanged

A single-bit Boolean that indicates whether the range variable changed since the last event was dispatched.

