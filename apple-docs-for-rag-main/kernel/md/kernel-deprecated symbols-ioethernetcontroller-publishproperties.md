

- Kernel
- Deprecated Symbols
- IOEthernetController
-  publishProperties 

# publishProperties

Publishes Ethernet controller properties and capabilities.

``` source
virtual bool publishProperties(); 
```

## Return Value

Returns true if all properties and capabilities were discovered, and published successfully, false otherwise. Returning false will prevent client objects from attaching to the Ethernet controller since a property that a client relies upon may be missing.

## Overview

This method publishes Ethernet controller properties to the property table. For instance, getHardwareAddress() is called to fetch the hardware address, and the address is then published to the property table. This method call is synchronized by the workloop's gate, and must never be called directly by subclasses.

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

