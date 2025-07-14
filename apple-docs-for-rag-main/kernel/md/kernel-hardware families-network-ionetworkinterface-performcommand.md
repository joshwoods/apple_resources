

- Kernel
- Hardware Families
- Network
- IONetworkInterface
-  performCommand 

# performCommand

Handles an ioctl command sent to the network interface.

``` source
virtual SInt32 performCommand( 
 IONetworkController *controller, 
 unsigned longcmd, 
 void *arg0, 
 void *arg1 ); 
```

## Parameters 

`controller`  

The controller object.

`cmd`  

The ioctl command code.

`arg0`  

Command argument 0. Generally a pointer to an ifnet structure associated with the interface.

`arg1`  

Command argument 1.

## Return Value

Returns a BSD return value defined in `bsd/sys/errno.h`.

## Overview

This method handles socket ioctl commands sent to the network interface from DLIL. IONetworkInterface handles commands that are common for all network interface types. A subclass of IONetworkInterface may override this method to override the command handling in IONetworkInterface, or to extend the command processing to handle additional commands. The ioctl commands handled by IONetworkInterface are `SIOCGIFMTU` (Get interface MTU size), `SIOCSIFMTU` (Set interface MTU size), `SIOCSIFMEDIA` (Set media), and `SIOCGIFMEDIA` (Get media and link status).

## See Also

### Miscellaneous

addNetworkData

Adds an `IONetworkData` object to the interface.

attachToDataLinkLayer

Attach the network interface to the BSD data link layer.

clearInputQueue

Discards all packets in the input queue.

controllerDidChangePowerState

Handles a notification that the network controller servicing this interface object has transitioned to a new power state.

controllerDidOpen

Sends a notification that the interface has opened the network controller.

controllerWillChangePowerState

Handles a notification that the network controller servicing this interface object will transition to a new power state.

controllerWillClose

Sends a notification that the interface will close the network controller.

debuggerRegistered

Tells the `IONetworkData` that this interface will be used by the debugger.

detachFromDataLinkLayer

Detach the network interface from the BSD data link layer.

feedPacketInputTap

Feed received packets to the BPF

feedPacketOutputTap

Feed output packets to the BPF

flushInputQueue

Submit all packets held in the input queue to the network stack.

free

Frees the `IONetworkInterface` object.

getController

Gets the `IONetworkController` object that created this interface.

getExtraFlags

Gets the current interface eflags.

getFlags

Gets the current interface flags.

getIfnet

Returns the `ifnet_t` allocated by the interface object.

getInterfaceState

Reports the current state of the interface object.

getInterfaceType

Gets the interface type.

getMaxTransferUnit

Gets the maximum transfer unit for this interface.

getMediaAddressLength

Gets the size of the media (MAC-layer) address.

getMediaHeaderLength

Gets the size of the media header.

getNamePrefix

Returns the BSD name prefix as a C-string.

getNetworkData(const char *)

Gets an `IONetworkData` object from the interface.

getNetworkData(const OSSymbol *)

Gets an `IONetworkData` object from the interface.

getUnitNumber

Gets the unit number assigned to this interface object.

handleClientClose

Handles a client close on the interface.

handleClientOpen

Handles a client open on the interface.

init

Initializes the `IONetworkInterface` object.

initIfnetParams

Allows a subclass to provide ifnet initialization parameters specific to an interface type.

inputEvent

Sends an event to the network stack.

inputPacket

For drivers to submit a received packet to the network stack.

isPrimaryInterface

Queries whether the interface is the primary network interface on the system.

isRegistered

Queries if the interface has attached to the BSD network stack.

lock

Acquires a recursive lock owned by the interface.

powerStateDidChangeTo

Handles a post-change power interest notification from the network controller.

powerStateWillChangeTo

Handles a pre-change power interest notification from the network controller.

registerOutputHandler

Registers a target/action to handle outbound packets.

removeNetworkData(const char *)

Removes an `IONetworkData` object from the interface.

removeNetworkData(const OSSymbol *)

Removes an `IONetworkData` object from the interface.

setFlags

Performs a read-modify-write operation on the current interface flags value.

setInterfaceState

Updates the interface object state flags.

setInterfaceType

Sets the interface type.

setMaxTransferUnit

Sets the maximum transfer unit for this interface.

setMediaAddressLength

Sets the size of the media (MAC-layer) address.

setMediaHeaderLength

Sets the size of the media header.

setUnitNumber

Assigns an unique unit number to this interface.

unlock

Releases the recursive lock owned by the interface.

