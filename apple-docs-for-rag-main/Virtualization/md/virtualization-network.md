

- Virtualization
-  Network 

API Collection

# Network

Configure the devices that connect the guest system to the network.

## Topics

### Configurations

class VZVirtioNetworkDeviceConfiguration

A configuration object that requests the creation of a network device for the guest system.

class VZNetworkDeviceConfiguration

The common configuration traits for network devices.

class VZMACAddress

The media access control (MAC) address for a network interface in your virtual machine.

### Attachment points

class VZBridgedNetworkDeviceAttachment

A network device that interacts directly with a physical network interface on the host computer.

class VZFileHandleNetworkDeviceAttachment

A network device that transmits raw network packets and frames using a datagram socket.

class VZNATNetworkDeviceAttachment

A device that routes network requests through the host computer and performs network address translation on the resulting packets.

class VZNetworkDeviceAttachment

The common behaviors for the network attachment points of your virtual machine.

### Hardware interfaces

class VZBridgedNetworkInterface

An object that identifies the supported network interfaces of the host computer.

### Devices

class VZNetworkDevice

A base class that represents a network device in a virtual machine.

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

Randomization

Configure a device for the guest system to use to generate random numbers.

Serial ports

Configure the serial devices that you use to communicate with the guest system.

Shared directories

Configure devices that share directories from the host into the guest system.

Sockets

Configure a device that manages port-based communication with the guest system.

Storage

Configure the block-storage devices that represent the disks of the guest system.

Consoles

Configure a device that manages multiport console communication with the guest system.

Clipboard sharing

Share the pasteboard between the host and guest system.

USB Devices

