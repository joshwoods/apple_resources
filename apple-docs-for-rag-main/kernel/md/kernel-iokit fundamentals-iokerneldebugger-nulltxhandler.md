

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  nullTxHandler 

# nullTxHandler

Null transmit handler.

``` source
static void nullTxHandler(
 IOService *target, 
 void *buffer, 
 UInt32 length ); 
```

## Overview

This function is registered as the transmit handler when an IOKernelDebugger object surrenders its status as the active debugger nub. Until another IOKernelDebugger object gets promoted, this function will handle polled transmit requests from KDP. This function does nothing useful.

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

nullRxHandler

Null receive handler.

nullSetModeHandler

Null set mode handler.

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

