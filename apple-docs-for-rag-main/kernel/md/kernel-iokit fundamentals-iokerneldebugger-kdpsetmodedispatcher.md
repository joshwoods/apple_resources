

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  kdpSetModeDispatcher 

# kdpSetModeDispatcher

The KDP set mode dispatch function.

``` source
static boolean_t kdpSetModeDispatcher(
 boolean_tactive); 
```

## Parameters 

`active`  

TRUE if entering KDP. FALSE if leaving KDP.

## Return Value

Return TRUE if the link is up and data can be sent/received. Otherwise, return FALSE.

## Overview

Field KDP set mode requests, then dispatches the call to the registered set mode handler.

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

