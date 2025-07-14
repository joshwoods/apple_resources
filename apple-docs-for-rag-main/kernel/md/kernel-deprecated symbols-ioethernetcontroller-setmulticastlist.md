

- Kernel
- Deprecated Symbols
- IOEthernetController
-  setMulticastList 

# setMulticastList

Sets the list of multicast addresses a multicast filter should use to match against the destination address of an incoming frame.

``` source
virtual IOReturn setMulticastList(
 IOEthernetAddress *addrs, 
 UInt32count); 
```

## Parameters 

`addrs`  

An array of Ethernet addresses. This argument must be ignored if the count argument is 0.

`count`  

The number of Ethernet addresses in the list. This value will be zero when the list becomes empty.

## Return Value

Returns kIOReturnUnsupported. Drivers must return kIOReturnSuccess to indicate success, or an error return code otherwise.

## Overview

This method sets the list of multicast addresses that the multicast filter should use to match against the destination address of an incoming frame. The frame should be accepted when a match occurs. Called when the multicast group membership of an interface object is changed. Drivers that support kIOPacketFilterMulticast should override this method and update the hardware multicast filter using the list of Ethernet addresses provided. Perfect multicast filtering is preferred if supported by the hardware, in order to reduce the number of unwanted packets received. If the number of multicast addresses in the list exceeds what the hardware is capable of supporting, or if perfect filtering is not supported, then ideally the hardware should be programmed to perform imperfect filtering, through some form of hash filtering mechanism. Only as a last resort should the driver enable reception of all multicast packets to satisfy this request. This method is called from the workloop context, and only if the driver reports kIOPacketFilterMulticast support in getPacketFilters().

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

setMulticastMode

Enables or disables multicast mode.

setPromiscuousMode

Enables or disables promiscuous mode.

setVlanTag

Encode a received packet with the vlan tag result reported by the hardware.

setWakeOnMagicPacket

Enables or disables the wake on Magic Packet support.

