

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  nullRxHandler 

# nullRxHandler

Null receive handler.

``` source
static void nullRxHandler(
 IOService *target, 
 void *buffer, 
 UInt32 *length, 
 UInt32 timeout ); 
```

## Overview

This function is registered as the receive handler when an IOKernelDebugger object surrenders its status as the active debugger nub. Until another IOKernelDebugger object gets promoted, this function will handle polled receive requests from KDP. This function does nothing except to log a warning message.

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

lock

Takes the debugger lock conditionally.

nullLinkStatusHandler

Null link status handler.

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

