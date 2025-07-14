

- Kernel
- IOKit Fundamentals
- IOKernelDebugger
-  powerStateDidChangeTo 

# powerStateDidChangeTo

Handles notification that the network controller did change power state.

``` source
virtual IOReturn powerStateDidChangeTo(
 IOPMPowerFlagsflags, 
 unsigned longstateNumber, 
 IOService *policyMaker ); 
```

## Parameters 

`flags`  

Description of the capability of the controller in the new power state.

`stateNumber`  

The number of the state in the state array that the controller is switching to.

`policyMaker`  

The policy maker that manages the controller's power state.

## Return Value

Returns the constant 3000000, to indicate a maximum of 3 seconds for the preparation to complete, and an acknowledgement delivered to the policy maker.

## Overview

If the controller became usable, then the controller is re-enabled, and the controller's handlers are re-registered.

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

powerStateWillChangeTo

Handles notification that the network controller will change power state.

registerHandler

Registers the target and the handler functions.

signalDebugger

Signal the kernel to enter the debugger when safe.

unlock

Releases the debugger lock.

