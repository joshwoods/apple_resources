

- Kernel
- Deprecated Symbols
- IOHIDEventService
-  handleClose 

# handleClose

Handle a client close on the interface.

``` source
virtual void handleClose(
 IOService *client,
 IOOptionBitsoptions); 
```

## Parameters 

`client`  

The client object that requested the close.

`options`  

Options passed to IOService::close().

## Overview

This method is called by IOService::close() with the arbitration lock held. This method will in turn call handleClientClose() to notify interested subclasses about the client close. If this represents the last close, then the interface will also close the controller before this method returns. The controllerWillClose() method will be called before closing the controller. Subclasses should not override this method.

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

handleIsOpen

Query whether a client has an open on the interface.

handleOpen

Handle a client open on the interface.

handleStart

Prepare the hardware and driver to support I/O operations.

handleStop

Quiesce the hardware and stop the driver.

