

- Kernel
- Deprecated Symbols
- IOEthernetController
-  enablePacketFilter 

# enablePacketFilter

Enables one of the supported packet filters from the given filter group.

``` source
virtual IOReturn enablePacketFilter(
 const OSSymbol *group, 
 UInt32 aFilter, 
 UInt32 enabledFilters, 
 IOOptionBits options = 0); 
```

## Parameters 

`group`  

The name of the filter group containing the filter to be enabled.

`aFilter`  

The filter to enable.

`enabledFilters`  

All filters currently enabled by the client.

`options`  

Optional flags for the enable request.

## Return Value

Returns the value returned by setMulticastMode() or setPromiscuousMode() if either of those two methods are called. Returns kIOReturnSuccess if the filter specified is kIOPacketFilterUnicast or kIOPacketFilterBroadcast. Returns kIOReturnUnsupported if the filter group specified is not gIONetworkFilterGroup.

## Overview

The default implementation of the abstract method inherited from IONetworkController. This method will call setMulticastMode() or setPromiscuousMode() when the multicast or the promiscuous filter is to be enabled. Requests to disable the Unicast or Broadcast filters are handled silently, without informing the subclass. Subclasses can override this method to change this default behavior, or to extend it to handle additional filter types or filter groups. This method call is synchronized by the workloop's gate.

## See Also

### Miscellaneous

createInterface

Creates an IOEthernetInterface object.

disablePacketFilter

Disables a packet filter that is currently enabled from the given filter group.

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

setVlanTag

Encode a received packet with the vlan tag result reported by the hardware.

setWakeOnMagicPacket

Enables or disables the wake on Magic Packet support.

