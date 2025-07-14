

- Kernel
- Deprecated Symbols
- IOHIDEventService
-  handleIsOpen 

# handleIsOpen

Query whether a client has an open on the interface.

``` source
virtual bool handleIsOpen(
 const IOService *client) const; 
```

## Return Value

true if the specified client, or any client if none (0) is specified, presently has an open on this object.

## Overview

This method is always called by IOService with the arbitration lock held. Subclasses should not override this method.

## See Also

### Miscellaneous

dispatchDigitizerEvent

Dispatch tablet events without orientation

dispatchDigitizerEventWithPolarOrientation

Dispatch tablet events with polar orientation

dispatchDigitizerEventWithTiltOrientation

Dispatch tablet events with tilt orientation

dispatchMultiAxisPointerEvent

Dispatch multi-axis pointer event

handleClose

Handle a client close on the interface.

handleOpen

Handle a client open on the interface.

handleStart

Prepare the hardware and driver to support I/O operations.

handleStop

Quiesce the hardware and stop the driver.

