

- Kernel
- Deprecated Symbols
- IOHIDEventService
-  handleStart 

# handleStart

Prepare the hardware and driver to support I/O operations.

``` source
virtual bool handleStart(
 IOService *provider ); 
```

## Parameters 

`provider`  

The provider argument passed to start().

## Return Value

True on success, or false otherwise. Returning false will cause start() to fail and return false.

## Overview

IOHIDEventService will call this method from start() before any I/O operations are issued to the concrete subclass. Methods such as getReportElements() are only called after handleStart() has returned true. A subclass that overrides this method should begin its implementation by calling the version in super, and then check the return value.

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

handleStop

Quiesce the hardware and stop the driver.

