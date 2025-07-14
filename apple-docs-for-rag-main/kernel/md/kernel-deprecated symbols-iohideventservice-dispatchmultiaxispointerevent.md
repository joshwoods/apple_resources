

- Kernel
- Deprecated Symbols
- IOHIDEventService
-  dispatchMultiAxisPointerEvent 

# dispatchMultiAxisPointerEvent

Dispatch multi-axis pointer event

``` source
virtual void dispatchMultiAxisPointerEvent( 
 AbsoluteTime timeStamp, 
 UInt32 buttonState, 
 IOFixed x, 
 IOFixed y, 
 IOFixed z, 
 IOFixed rX = 0, 
 IOFixed rY = 0, 
 IOFixed rZ = 0, 
 IOOptionBits options = 0 ); 
```

## Parameters 

`timeStamp`  

AbsoluteTime representing origination of event

`buttonState`  

Button mask where bit0 is the primary button, bit1 secondary and so forth

`x`  

Absolute location of pointer along the x-axis from -1.0 to 1.0 in 16:16 fixed point.

`y`  

Absolute location of pointer along the y-axis from -1.0 to 1.0 in 16:16 fixed point.

`z`  

Absolute location of pointer along the z-axis from -1.0 to 1.0 in 16:16 fixed point.

`rX`  

Absolute rotation of pointer around the x-axis from -1.0 to 1.0 in 16:16 fixed point.

`rY`  

Absolute rotation of pointer around the y-axis from -1.0 to 1.0 in 16:16 fixed point.

`rZ`  

Absolute rotation of pointer around the z-axis from -1.0 to 1.0 in 16:16 fixed point.

`options`  

Additional options to be used when dispatching event such as leveraging rotational axis for translation or using the z axis for vertical scrolling.

## Overview

This is meant to be used with joysticks or multi-axis pointer devices such as those with with 6 degrees of freedom. This function will generate related relative pointer and scroll event associated with movement.

## See Also

### Miscellaneous

dispatchDigitizerEvent

Dispatch tablet events without orientation

dispatchDigitizerEventWithPolarOrientation

Dispatch tablet events with polar orientation

dispatchDigitizerEventWithTiltOrientation

Dispatch tablet events with tilt orientation

handleClose

Handle a client close on the interface.

handleIsOpen

Query whether a client has an open on the interface.

handleOpen

Handle a client open on the interface.

handleStart

Prepare the hardware and driver to support I/O operations.

handleStop

Quiesce the hardware and stop the driver.

