

- HIDDriverKit
- IOHIDDigitizerStylusData
-  invert 

Instance Property

# invert

A single-bit Boolean that indicates whether the stylus is inverted.

DriverKitmacOS

``` source
uint32_t invert;
```

## See Also

### Getting the Stylus Data

identifier

A unique stylus identifier.

x

An x-axis value in the range `0.0` to `1.0`.

y

A y-axis value in the range `0.0` to `1.0`.

tipPressure

A tip pressure value in the range `0.0` to `1.0`.

barrelPressure

The barrel pressure value in the range `0.0` to `1.0`.

tiltX

The tilt of the stylus across the x-axis.

tiltY

The tilt of the stylus across the y-axis.

twist

The clockwise rotation of the stylus.

pointerType

An optional pointer type defined by vendor.

effect

An optional stylus effect defined by vendor.

uniqueID

An optional unique identifier for the stylus.

inRange

A single-bit Boolean that indicates whether the stylus is in range.

tip

A single-bit Boolean that indicates whether the tip of the stylus is in contact with the surface of the digitizer.

barrelSwitch

A single-bit Boolean that indicates whether the barrel switch button is pressed.

eraser

A Boolean value that indicates whether the inverted stylus is in contact with the surface of the digitizer.

