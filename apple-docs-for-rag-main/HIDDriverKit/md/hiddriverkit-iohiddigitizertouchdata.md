

- HIDDriverKit
-  IOHIDDigitizerTouchData 

Structure

# IOHIDDigitizerTouchData

A structure containing the current digitizer touch data.

DriverKitmacOS

``` source
typedef struct IOHIDDigitizerTouchData { ... } IOHIDDigitizerTouchData;
```

## Overview

Pass this structure to the dispatchDigitizerTouchEvent method when dispatching touch events.

## Topics

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

touchChanged

A single-bit Boolean that indicates whether the touch variable changed since the last event was dispatched.

positionChanged

A single-bit Boolean that indicates whether the x or y position changed since the last event was dispatched.

rangeChanged

A single-bit Boolean that indicates whether the range variable changed since the last event was dispatched.

## See Also

### Events

IOHIDDigitizerStylusData

A structure containing digitizer stylus data.

