

- Kernel
- IOKit Fundamentals
-  IOKernelDebugger 

Class

# IOKernelDebugger

Kernel debugger nub.

macOS 10.0+

``` source
class IOKernelDebugger : IOService
```

## Overview

This object interfaces with the KDP (kernel debugger protocol) module and dispatches KDP requests to its target (provider). The target, designated as the debugger device, must implement a pair of handler functions that are called to handle KDP transmit and receive requests during a debugging session. Only a single IOKernelDebugger in the system can be active at a given time. The active IOKernelDebugger is the one that has an IOKDP object attached as a client.

The debugger device is usually a subclass of IOEthernetController. However, any IOService can service an IOKernelDebugger client, implement the two polled mode handlers, and transport the KDP packets through a data channel. However, KDP assumes that the debugger device is an Ethernet interface and therefore it will always send, and expect to receive, an Ethernet frame.

## Topics

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

registerHandler

Registers the target and the handler functions.

signalDebugger

Signal the kernel to enter the debugger when safe.

unlock

Releases the debugger lock.

### Instance Variables

_reserved

### Instance Methods

- free

- getMetaClass

- handleClose

- handleIsOpen

- handleOpen

- init

- message

- powerStateDidChangeTo

- powerStateWillChangeTo

### Type Methods

+ debugger

+ interfacePublished

+ kdpLinkStatusDispatcher

+ kdpReceiveDispatcher

+ kdpSetModeDispatcher

+ kdpTransmitDispatcher

+ lock

+ nullLinkStatusHandler

+ nullRxHandler

+ nullSetModeHandler

+ nullTxHandler

+ registerHandler

+ signalDebugger

+ unlock

## Relationships

### Inherits From

- IOService

## See Also

### Debugging

IOKitDiagnostics

IOKitDiagnosticsParameters

