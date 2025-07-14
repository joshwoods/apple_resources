

- Kernel
- Hardware Families
- Network
- IONetworkController
-  selectMediumWithName 

# selectMediumWithName

A client request to change the medium selection.

``` source
virtual IOReturn selectMediumWithName(
 const OSSymbol *mediumName); 
```

## Parameters 

`mediumName`  

An OSSymbol object that describes the name of the new medium selected by the client.

## Return Value

Returns the return from selectMedium() if a matching entry was found from the medium dictionary. Returns kIOReturnUnsupported if a medium dictionary does not exist, or kIOReturnBadArgument if the name given does not match any entry in the medium dictionary.

## Overview

This method is called when a client issues a command for the controller to change its current medium selection. This implementation will look for an entry in the medium dictionary published by the driver that is associated with the key given. If a match is found, then selectMedium() is called to perform the selection, otherwise an error is reported back to the client. Subclasses should override selectMedium() and not this method. This method call is synchronized by the workloop's gate.

## See Also

### Miscellaneous

allocatePacket

Allocates a packet with a data buffer that is larger than or equal to the size specified.

attachDebuggerClient

Attaches a new IOKernelDebugger client object.

attachInterface

Attaches a new network interface client object.

configureInterface

Configures a newly created network interface object.

copyMediumDictionary

Returns a copy of the medium dictionary published by the driver.

copyPacket

Allocates a new packet, containing data copied from an existing source packet.

createInterface

Creates a new network interface object.

createOutputQueue

Creates an IOOutputQueue to handle output packet queueing, and also to resolve contention for the controller's transmitter from multiple client threads.

createWorkLoop

Method called by IONetworkController prior to the initial getWorkLoop() call.

detachDebuggerClient

Detaches an IOKernelDebugger client object.

detachInterface

Detaches an interface client object.

disable

A disable request from an IOKernelDebugger client.

disable(IONetworkInterface *)

A request from an interface client to disable the controller.

disable(IOService *)

Handles a disable request from a client.

disablePacketFilter

Disables a packet filter that is currently enabled from the given filter group.

doDisable

Makes a synchronized call to disable() through executeCommand().

doEnable

Makes a synchronized call to enable() through executeCommand().

enable

An enable request from an IOKernelDebugger client.

enable(IONetworkInterface *)

A request from an interface client to enable the controller.

enable(IOService *)

Handles an enable request from a client.

enablePacketFilter

Enables one of the supported packet filters from the given filter group.

executeCommand

Makes a C function call through the command gate.

free

Frees the IONetworkController object.

freePacket

Releases the packet given back to the free pool.

getChecksumDemand

Fetches the demand for hardware checksum computation and insertion for the given packet before it is transmitted on the network.

getChecksumSupport

Gets checksums that are supported by the network controller for the given checksum family.

getCommandClient

Gets the command client object.

getCommandGate

Gets the IOCommandGate object created by IONetworkController.

getDebuggerLinkStatus

Debugger polled-mode link status handler.

getFeatures

Reports generic features supported by the controller and/or the driver.

getHardwareAddress

Gets the network controller's permanent hardware/station address.

getMaxPacketSize

Gets the maximum packet size supported by the controller.

getMediumDictionary

Returns the medium dictionary published by the driver.

getMinPacketSize

Gets the minimum packet size supported by the controller.

getOutputHandler

Gets the address of the method designated to handle output packets for the network controller.

getOutputQueue

Gets the IOOutputQueue object created by createOutputQueue().

getPacketBufferConstraints

Gets the controller's packet buffer constraints.

getPacketFilters

Gets the set of packet filters supported by the network controller for the given filter group.

getSelectedMedium

Gets the current selected medium.

handleClose

Handles a client close.

handleIsOpen

Queries whether a client has an open on the controller.

handleOpen

Handles a client open.

init

Initializes the IONetworkController object.

message

Receives messages delivered from an attached provider.

newModelString

newRevisionString

newVendorString

outputPacket

Transmits an output packet.

prepare

Prepares the controller before an IOService is created and attached as a client.

publishMediumDictionary

Publishes a dictionary of IONetworkMedium objects to advertise the media selection supported by the network controller.

publishProperties

Publishes controller properties and capabilities.

receivePacket

Debugger polled-mode receive handler.

registerWithPolicyMaker

Implemented by controller drivers to register with the power management policy-maker.

releaseDebuggerLock

Releases the global debugger lock.

releaseFreePackets

Releases all packets held in the free packet queue.

replaceOrCopyPacket

A helper method that combines the functionality of copyPacket() and replacePacket() to process a packet containing a received frame.

replacePacket

Allocates a new packet to replace an existing packet, the existing packet is then returned.

reserveDebuggerLock

Takes the global debugger lock.

selectMedium

A client request to change the medium selection.

sendPacket

Debugger polled-mode transmit handler.

setChecksumResult

Encodes a received packet with the checksum result reported by the hardware.

setDebuggerMode

Set debugger mode for network drivers.

setHardwareAddress

Sets or changes the station address used by the network controller.

setLinkStatus

Reports the link status and the active medium.

setMaxPacketSize

A client request to change the maximum packet size.

setSelectedMedium

Designates an entry in the published medium dictionary as the current selected medium.

start

Starts the network controller.

stop

Stops the network controller.

systemWillShutdown

Handles system shutdown and restart notifications.

