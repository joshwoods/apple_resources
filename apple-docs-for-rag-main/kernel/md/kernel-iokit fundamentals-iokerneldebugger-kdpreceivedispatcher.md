

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  kdpReceiveDispatcher 

# kdpReceiveDispatcher

The KDP receive dispatch function.

``` source
static void kdpReceiveDispatcher(
 void *buffer, 
 UInt32 *length, 
 UInt32timeout); 
```

## Parameters 

`buffer`  

KDP receive buffer. The buffer allocated by KDP has room for 1518 bytes. The receive handler must not overflow this buffer.

`length`  

The amount of data received and placed into the buffer. Set to 0 if a frame was not received during the poll interval.

`timeout`  

The amount of time to poll in milliseconds while waiting for a frame to arrive.

## Overview

Field KDP receives requests, then dispatches the call to the registered receiver handler.

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

