

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  lock 

# lock

Takes the debugger lock conditionally.

``` source
static IODebuggerLockState lock(
 IOService *target ); 
```

## Parameters 

`target`  

The target or provider of an IOKernelDebugger object.

## Return Value

Returns kIODebuggerLockTaken if the lock was taken, or 0 otherwise.

## Overview

This method takes the debugger lock if the object given matches the target registered by registerHandler().

## See Also

### Miscellaneous

debugger

Factory method that performs allocation and initialization of an IOKernelDebugger object.

free

Frees the IOKernelDebugger instance.

handleClose

Handles a client close.

handleIsOpen

Queries whether a client has an open on this object.

handleOpen

Handles a client open.

init

Initializes an IOKernelDebugger instance.

kdpLinkStatusDispatcher

The KDP link status dispatch function.

kdpReceiveDispatcher

The KDP receive dispatch function.

kdpSetModeDispatcher

The KDP set mode dispatch function.

kdpTransmitDispatcher

The KDP transmit dispatch function.

nullLinkStatusHandler

Null link status handler.

nullRxHandler

Null receive handler.

nullSetModeHandler

Null set mode handler.

nullTxHandler

Null transmit handler.

powerStateDidChangeTo

Handles notification that the network controller did change power state.

powerStateWillChangeTo

Handles notification that the network controller will change power state.

registerHandler

Registers the target and the handler functions.

signalDebugger

Signal the kernel to enter the debugger when safe.

unlock

Releases the debugger lock.

