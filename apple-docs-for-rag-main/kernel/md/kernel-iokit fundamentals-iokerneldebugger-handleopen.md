

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  handleOpen 

# handleOpen

Handles a client open.

``` source
virtual bool handleOpen(
 IOService *forClient, 
 IOOptionBitsoptions, 
 void *arg ); 
```

## Parameters 

`forClient`  

The client (IOKDP) requesting the open.

`options`  

Options passed to the open() call. Not used.

`arg`  

A family defined argument passed to the open() call. Not used.

## Return Value

Returns true on success, false otherwise.

## Overview

This method is called by IOService::open() to handle an open from a client (IOKDP) with the arbitration lock held.

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

