

- Kernel
- Deprecated Symbols
- IOEthernetController
-  getHardwareAddress(void \*, UInt32 \*) 

# getHardwareAddress(void \*, UInt32 \*)

Gets the Ethernet controller's station address.

``` source
virtual IOReturn getHardwareAddress(
 void *addr, 
 UInt32 *inOutAddrBytes); 
```

## Parameters 

`addr`  

The buffer where the controller's hardware address should be written.

`inOutAddrBytes`  

The size of the address buffer provided by the client, and replaced by this method with the actual size of the hardware address in bytes.

## Return Value

Returns kIOReturnSuccess on success, or an error otherwise.

## Overview

The default implementation of the abstract method inherited from IONetworkController. This method will call the overloaded form IOEthernetController::getHardwareAddress() that subclasses are expected to override.

## See Also

### Miscellaneous

createInterface

Creates an IOEthernetInterface object.

disablePacketFilter

Disables a packet filter that is currently enabled from the given filter group.

enablePacketFilter

Enables one of the supported packet filters from the given filter group.

free

Frees the IOEthernetController instance.

getHardwareAddress(IOEthernetAddress *)

Gets the Ethernet controller's permanent station address.

getMaxPacketSize

Gets the maximum packet size supported by the Ethernet controller, including the frame header and FCS.

getMinPacketSize

Gets the minimum packet size supported by the Ethernet controller, including the frame header and FCS.

getPacketFilters(const OSSymbol *, UInt32 *)

Gets the set of packet filters supported by the Ethernet controller in the given filter group.

getPacketFilters(UInt32 *)

Gets the set of packet filters supported by the Ethernet controller in the network filter group.

getVlanTagDemand

Fetch the demand for hardware vlan tag stuffing for the given packet before it is transmitted on the network.

init

Initializes an IOEthernetController object.

initialize

IOEthernetController class initializer.

publishProperties

Publishes Ethernet controller properties and capabilities.

setHardwareAddress(const IOEthernetAddress *)

Sets or changes the station address used by the Ethernet controller.

setHardwareAddress(const void *, UInt32)

Sets or changes the station address used by the Ethernet controller.

setMulticastList

Sets the list of multicast addresses a multicast filter should use to match against the destination address of an incoming frame.

setMulticastMode

Enables or disables multicast mode.

setPromiscuousMode

Enables or disables promiscuous mode.

setVlanTag

Encode a received packet with the vlan tag result reported by the hardware.

setWakeOnMagicPacket

Enables or disables the wake on Magic Packet support.

