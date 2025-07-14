

- HIDDriverKit
-  IOHIDDigitizerStylusData 

Structure

# IOHIDDigitizerStylusData

A structure containing digitizer stylus data.

DriverKitmacOS

``` source
typedef struct IOHIDDigitizerStylusData { ... } IOHIDDigitizerStylusData;
```

## Overview

When dispatching stylus events, allocate an `IOHIDDigitizerStylusData` structure, fill it with stylus data, and pass it to the dispatchDigitizerStylusEvent method.

## Topics

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

invert

A single-bit Boolean that indicates whether the stylus is inverted.

eraser

A Boolean value that indicates whether the inverted stylus is in contact with the surface of the digitizer.

tipChanged

A single-bit Boolean that indicates whether the tip contact status changed since the last event was dispatched.

positionChanged

A single-bit Boolean that indicates whether the x or y position changed since the last event was dispatched.

rangeChanged

A single-bit Boolean that indicates whether the in-range status changed since the last event was dispatched.

## See Also

### Events

IOHIDDigitizerTouchData

A structure containing the current digitizer touch data.

