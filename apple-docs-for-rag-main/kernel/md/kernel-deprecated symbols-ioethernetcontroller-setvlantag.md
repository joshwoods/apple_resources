

- Kernel
- Deprecated Symbols
- IOEthernetController
-  setVlanTag 

# setVlanTag

Encode a received packet with the vlan tag result reported by the hardware.

``` source
virtual void setVlanTag(
 mbuf_tm,
 UInt32vlanTag); 
```

## Parameters 

`m`  

A mbuf containing a packet that has had its 802.1q vlan tag stripped by the hardware.

`vlanTag`  

A value in host order that contains the 802.1q vlan tag and priority in the low order 16 bits. The hi order word is currently unused and should be set to 0.

## Overview

A network controller that can strip 802.1Q vlan tag information for a received packet should call this method to encode the result on the packet, before passing it up towards the protocol stacks.

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

setMulticastList

Sets the list of multicast addresses a multicast filter should use to match against the destination address of an incoming frame.

setMulticastMode

Enables or disables multicast mode.

setPromiscuousMode

Enables or disables promiscuous mode.

setWakeOnMagicPacket

Enables or disables the wake on Magic Packet support.

