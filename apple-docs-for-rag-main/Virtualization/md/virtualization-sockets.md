

- Virtualization
-  Sockets 

API Collection

# Sockets

Configure a device that manages port-based communication with the guest system.

## Topics

### Configurations

class VZVirtioSocketDeviceConfiguration

A configuration object that requests the creation of a socket device to communicate with the guest system.

class VZSocketDeviceConfiguration

The common configuration traits for socket device requests.

### Devices

class VZVirtioSocketDevice

A device that manages port-based connections between the guest system and the host computer.

class VZSocketDevice

The common behavior of socket devices.

### Connection management

class VZVirtioSocketListener

An object that listens for port-based connection requests from the guest operating system.

class VZVirtioSocketConnection

A port-based connection between the guest operating system and the host computer.

## See Also

### Devices

Audio

Configure audio devices that enable the guest operating system to perform audio playback and capture through the host’s audio devices.

Graphics

Configure a device for a guest to display its UI.

Keyboards and pointing devices

Configure devices that connect a mouse and keyboard to the guest system.

Memory

Configure a memory balloon device to change the allocated memory for the guest system.

Network

Configure the devices that connect the guest system to the network.

Randomization

Configure a device for the guest system to use to generate random numbers.

Serial ports

Configure the serial devices that you use to communicate with the guest system.

Shared directories

Configure devices that share directories from the host into the guest system.

Storage

Configure the block-storage devices that represent the disks of the guest system.

Consoles

Configure a device that manages multiport console communication with the guest system.

Clipboard sharing

Share the pasteboard between the host and guest system.

USB Devices

