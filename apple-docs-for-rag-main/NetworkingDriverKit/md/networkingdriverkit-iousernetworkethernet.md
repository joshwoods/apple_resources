

- NetworkingDriverKit
-  IOUserNetworkEthernet 

Class

# IOUserNetworkEthernet

The object you use to manage the setup, configuration, and teardown of your networking driver.

DriverKit

``` source
class IOUserNetworkEthernet;
```

## Overview

Subclass `IOUserNetworkEthernet` and override the methods you need to implement your driver’s behavior. Your subclass manages your driver’s overall life cycle, and facilitates communication between the hardware and the rest of the system. Use the Start method to establish a link to your hardware and to create the data structures needed to manage incoming and outgoing data packets. Use the Stop method to clean up the data structures you create in your Start method.

Override other methods of this class, and of the IOService parent class, as needed to enable your interface and implement other network-related behaviors. For example, you might want to override the inherited setPowerState method to respond to power-level changes.

### Specify the Driver’s Personality Information

When you subclass `IOUserNetworkEthernet`, update the `IOKitPersonalities` key of your driver extension’s `Info.plist` file with information to match your driver to appropriate hardware. For this class, always include the keys and values in the following table.

| Key | Discussion |
|----|----|
| `IOClass` | The value IOUserNetworkEthernet. |
| `IOProviderClass` | The provider class information. For USB-based network interfaces, specify IOUSBHostInterface. |
| `IOUserClass` | The name of your custom subclass. |
| CFBundleIdentifier | The bundle identifier of your driver. |
| `CFBundleIdentifierKernel` | The value `com.apple.iokit.IOSkywalkFamily`. |

You may add other keys to assist with the matching process. For example, you might include the `bInterfaceClass`, `bInterfaceProtocol`, and `bInterfaceSubClass` keys to match against specific USB device attributes. The USB specification defines which keys to include when matching your driver to a USB device. For information about the specific key combinations, see *Universal Serial Bus Common Class Specification* at https://www.usb.org.

## Topics

### Configuring the Driver Service

init

Handles the basic initialization of the service.

free

Performs any final cleanup for the service.

RegisterEthernetInterface

Registers your driver with the networking stack.

### Declaring the Supported Media Types

ReportAvailableMediaTypes

Tells the system what types of networking media your driver supports.

SelectMediaType

Selects the media type to use when communicating with the network stack.

IOUserNetworkMediaType

A structure describing a specific Ethernet type and configuration that your driver supports.

### Enabling Your Service

SetInterfaceEnable

Enables or disables your service.

### Configuring Link Attributes

SetTxPacketHeadroom

Reserves the specified number of bytes at the front of each packet.

SetTxPacketTailroom

Reserves the specified number of bytes at the end of each packet.

SetSoftwareVlanSupport

Enables software VLAN support.

SetMulticastAddresses

Sets the device addresses to use for multicast filtering.

SetAllMulticastModeEnable

Enables or disables multicast support for your service.

SetPromiscuousModeEnable

Enables or disables support for monitoriong all network packets.

SetWakeOnMagicPacketSupport

Tells the system whether the device supports being woken up when a specially formatted packet arrives.

SetWakeOnMagicPacketEnable

Enables or disables support for waking up the device when a specially formatted packet arrives.

IOUserNetworkMACAddress

A hardware address for a device.

### Reporting the Connection Status

ReportLinkStatus

Reports the status of the link between the device and your driver to the system.

ReportLinkQuality

Reports the quality of the link between the device and your driver to the system.

ReportDataBandwidths

Reports the input and output bandwidth between the device and your driver to the system.

IOUserNetworkLinkStatus

A type for specifying the state of your device’s connection.

IOUserNetworkLinkQuality

A type for specifying the quality of your device’s connection to the host.

### Instance Methods

GetHardwareAssists

GetMaxTransferUnit

RegisterEthernetInterface

ReportNicProxyLimits

SetHardwareAssists

SetMTU

addHardwareCountsWithInterfaceStatistics

bpfAttach

bpfTap

bpfTapInputPacket

bpfTapOutputPacket

getBSDName

getBSDNamePrefix

getBSDUnitNumber

getFeatureFlags

getHardwareAddress

getHardwareAssists

getInitialMedia

getInterfaceSubFamily

getMaxTransferUnit

getSupportedMediaArray

getTSOOptions

getTxDataOffset

handleChosenMedia

hwConfigNicProxyData

hwConfigNicProxyData

processInterfaceCommand

registerEthernetInterface

registerEthernetInterface

reportDataBandwidths

reportLinkQuality

reportLinkStatus

reportNicProxyLimits

setAllMulticastModeEnable

setHardwareAddress

setHardwareAssists

setHardwareAssists

setInterfaceEnable

setMaxTransferUnit

setMulticastAddresses

setPowerState

setPromiscuousModeEnable

start

stop

updateInterfaceDescriptor

## Relationships

### Inherits From

- IOService

