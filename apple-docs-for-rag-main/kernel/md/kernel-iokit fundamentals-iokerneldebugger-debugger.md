

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  debugger 

# debugger

Factory method that performs allocation and initialization of an IOKernelDebugger object.

``` source
static IOKernelDebugger * debugger(
 IOService *target, 
 IODebuggerTxHandlertxHandler, 
 IODebuggerRxHandlerrxHandler, 
 IODebuggerLinkStatusHandlerlinkStatusHandler, 
 IODebuggerSetModeHandlersetModeHandler); 
```

## Parameters 

`target`  

The target object that implements the debugger handlers.

`txHandler`  

The target's transmit handler. A pointer to a 'C' function.

`rxHandler`  

The target's receive handler. A pointer to a 'C' function.

`linkStatusHandler`  

The target's link status handler. A pointer to a 'C' function.

`setModeHandler`  

The target's set mode handler. A pointer to a 'C' function.

## Return Value

Returns an IOKernelDebugger instance on success, 0 otherwise.

## See Also

### Miscellaneous

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

registerHandler

Registers the target and the handler functions.

signalDebugger

Signal the kernel to enter the debugger when safe.

unlock

Releases the debugger lock.

