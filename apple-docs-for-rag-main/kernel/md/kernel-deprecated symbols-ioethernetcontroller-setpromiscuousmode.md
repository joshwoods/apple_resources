

- Kernel
- Deprecated Symbols
- IOEthernetController
-  setPromiscuousMode 

# setPromiscuousMode

Enables or disables promiscuous mode.

``` source
virtual IOReturn setPromiscuousMode(
 boolactive); 
```

## Parameters 

`active`  

True to enable promiscuous mode, false to disable it.

## Return Value

Returns kIOReturnUnsupported. If overridden, drivers must return kIOReturnSuccess on success, or an error return code otherwise.

## Overview

Called by enablePacketFilter() or disablePacketFilter() when there is a change in the activation state of the promiscuous filter identified by kIOPacketFilterPromiscuous. This method is called from the workloop context.

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

setVlanTag

Encode a received packet with the vlan tag result reported by the hardware.

setWakeOnMagicPacket

Enables or disables the wake on Magic Packet support.

