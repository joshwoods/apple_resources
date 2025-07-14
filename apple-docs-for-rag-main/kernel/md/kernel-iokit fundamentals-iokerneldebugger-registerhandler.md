

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  registerHandler 

# registerHandler

Registers the target and the handler functions.

``` source
static void registerHandler(
 IOService *target, 
 IODebuggerTxHandler txHandler = 0, 
 IODebuggerRxHandler rxHandler = 0, 
 IODebuggerLinkStatusHandler linkUpHandler = 0, 
 IODebuggerSetModeHandler setModeHandler = 0); 
```

## Parameters 

`target`  

The target object.

`txHandler`  

The transmit handler function. The null handler is registered if the argument is zero.

`rxHandler`  

The receive handler function. The null handler is

`linkUpHandler`  

The linkup handler function. The null handler is registered if the argument is zero.

## Overview

This method is called by handleOpen() and handleClose() to register or unregister the target and its handler functions.

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

nullTxHandler

Null transmit handler.

powerStateDidChangeTo

Handles notification that the network controller did change power state.

powerStateWillChangeTo

Handles notification that the network controller will change power state.

signalDebugger

Signal the kernel to enter the debugger when safe.

unlock

Releases the debugger lock.

