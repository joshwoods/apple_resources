

- Kernel
- Deprecated Symbols
- IOEthernetController
-  getPacketFilters(const OSSymbol \*, UInt32 \*) 

# getPacketFilters(const OSSymbol \*, UInt32 \*)

Gets the set of packet filters supported by the Ethernet controller in the given filter group.

``` source
virtual IOReturn getPacketFilters(
 const OSSymbol *group, 
 UInt32 *filters) const; 
```

## Parameters 

`group`  

The name of the filter group.

`filters`  

Pointer to the mask of supported filters returned by this method.

## Return Value

Returns kIOReturnSuccess. Drivers that override this method must return kIOReturnSuccess to indicate success, or an error return code otherwise.

## Overview

The default implementation of the abstract method inherited from IONetworkController. When the filter group specified is gIONetworkFilterGroup, then this method will return a value formed by a bitwise OR of kIOPacketFilterUnicast, kIOPacketFilterBroadcast, kIOPacketFilterMulticast, kIOPacketFilterPromiscuous. Otherwise, the return value will be set to zero (0). Subclasses must override this method if their filtering capability differs from what is reported by this default implementation. This method is called from the workloop context, and the result is published to the I/O Kit Registry.

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

getHardwareAddress(void *, UInt32 *)

Gets the Ethernet controller's station address.

getMaxPacketSize

Gets the maximum packet size supported by the Ethernet controller, including the frame header and FCS.

getMinPacketSize

Gets the minimum packet size supported by the Ethernet controller, including the frame header and FCS.

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

