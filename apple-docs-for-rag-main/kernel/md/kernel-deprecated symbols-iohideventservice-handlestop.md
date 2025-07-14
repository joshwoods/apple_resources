

- Kernel
- Deprecated Symbols
- IOHIDEventService
-  handleStop 

# handleStop

Quiesce the hardware and stop the driver.

``` source
virtual void handleStop(
 IOService *provider ); 
```

## Parameters 

`provider`  

The provider argument passed to stop().

## Overview

IOHIDEventService will call this method from stop() to signal that the hardware should be quiesced and the driver stopped. A subclass that overrides this method should end its implementation by calling the version in super.

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

handleOpen

Handle a client open on the interface.

handleStart

Prepare the hardware and driver to support I/O operations.

