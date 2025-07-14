

- Kernel
- Deprecated Symbols
-  IOEthernetController Deprecated

Class

# IOEthernetController

Abstract superclass for Ethernet controllers.

macOS 10.6–10.15.4Deprecated

``` source
class IOEthernetController : IONetworkController
```

## Overview

Ethernet controller drivers should subclass IOEthernetController, and implement or override the hardware specific methods to create an Ethernet driver. An interface object (an IOEthernetInterface instance) must be instantiated by the driver, through attachInterface(), to connect the controller driver to the data link layer.

## Topics

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

setVlanTag

Encode a received packet with the vlan tag result reported by the hardware.

setWakeOnMagicPacket

Enables or disables the wake on Magic Packet support.

### Instance Variables

_reserved

### Instance Methods

- addTimeSyncReceivePacketHandler

- addTimeSyncTransmitPacketHandler

- allocateAVBPacket

- changeAVBControllerState

- cleanupTransmitQueue

- completeAVBPacket

- createInterface

- createRealtimeAVBPacketPool

- deregisterForAVBStateChangeNotifications

- disablePacketFilter

- enablePacketFilter

- free

- getAVBSupport

- getControllerAVBState

- getHardwareAddress

- getHardwareAddress

- getMaxPacketSize

- getMetaClass

- getMinPacketSize

- getPacketFilters

- getPacketFilters

- getRealtimeReceiveQueueFilter

- getTransmitQueuePacketLatency

- getTransmitQueuePrefetchDelay

- getVlanTagDemand

- init

- publishProperties

- receivedTimeSyncPacket

- registerForAVBStateChangeNotifications

- removeTimeSyncReceivePacketHandler

- removeTimeSyncTransmitPacketHandler

- setAVBControllerState

- setAVBPacketMapper

- setGPTPPresent

- setHardwareAddress

- setHardwareAddress

- setMulticastList

- setMulticastMode

- setNumberOfRealtimeReceiveQueues

- setNumberOfRealtimeTransmitQueues

- setPromiscuousMode

- setRealtimeMulticastIsAllowed

- setRealtimeReceiveDestinationMACList

- setRealtimeReceiveQueueFilter

- setRealtimeReceiveQueuePacketHandler

- setTimeSyncPacketSupport

- setTransmitQueuePacketLatency

- setTransmitQueuePrefetchDelay

- setVlanTag

- setWakeOnMagicPacket

- timeSyncCallbackThread

- transmitRealtimePackets

- transmitTimeSyncPacket

- transmittedTimeSyncPacket

### Type Methods

+ allocatedAVBPacketCompletion

+ initialize

+ realtimePoolAVBPacketCompletion

+ timeSyncCallbackThreadEntry

## Relationships

### Inherits From

- IONetworkController

## See Also

### IOKit

IOUSBDevice

An input/output service object that represents a device on the USB bus.

Deprecated

IOUSBInterface

An object that represents an interface of a device on the USB bus.

Deprecated

IOOFPathMatchingDeprecated

IOUSBHostInterfaceDeprecated

IOUSBHostDeviceDeprecated

IOUSBHostPipeDeprecated

IOUSBHostIOSourceDeprecated

IOUSBHostStreamDeprecated

IOHIDEventDriverDeprecated

IOHIDEventService

IOService represents an device or OS service in IOKit and DriverKit.

Deprecated

IOHIDInterface

IOService represents an device or OS service in IOKit and DriverKit.

Deprecated

IOHIDSystemDeprecated

IOHIKeyboardMapperDeprecated

IOHIKeyboardDeprecated

IOHIPointingDeprecated

IOHIDeviceDeprecated

IOHIDElementDeprecated

IOHIDWorkLoopDeprecated

IOEthernetInterface

The Ethernet interface object.

Deprecated

