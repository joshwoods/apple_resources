

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  kdpTransmitDispatcher 

# kdpTransmitDispatcher

The KDP transmit dispatch function.

``` source
static void kdpTransmitDispatcher(
 void *buffer,
 UInt32length); 
```

## Parameters 

`buffer`  

KDP transmit buffer. This buffer contains a KDP frame to be sent on the network.

`length`  

The number of bytes in the transmit buffer.

## Overview

Field KDP transmit requests, then dispatches the call to the registered transmit handler.

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

