

- Kernel
- Deprecated Symbols
- IOHIDEventService
-  handleOpen 

# handleOpen

Handle a client open on the interface.

``` source
virtual bool handleOpen(
 IOService *client, 
 IOOptionBitsoptions, 
 void *argument); 
```

## Parameters 

`client`  

The client object that requested the open.

`options`  

Options passed to IOService::open().

`argument`  

Argument passed to IOService::open().

## Return Value

true to accept the client open, false otherwise.

## Overview

This method is called by IOService::open() with the arbitration lock held, and must return true to accept the client open. This method will in turn call handleClientOpen() to qualify the client requesting the open.

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

handleIsOpen

Query whether a client has an open on the interface.

handleStart

Prepare the hardware and driver to support I/O operations.

handleStop

Quiesce the hardware and stop the driver.

