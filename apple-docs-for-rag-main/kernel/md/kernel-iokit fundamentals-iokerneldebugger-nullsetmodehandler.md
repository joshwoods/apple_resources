

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  nullSetModeHandler 

# nullSetModeHandler

Null set mode handler.

``` source
static bool nullSetModeHandler(
 IOService *target,
 bool active); 
```

## Return Value

This function will always return true.

## Overview

This function is registered as the set mode handler when an IOKernelDebugger object surrenders its status as the active debugger nub. Until another IOKernelDebugger object gets promoted, this function will handle set mode requests from KDP.

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

