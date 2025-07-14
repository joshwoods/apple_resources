

- Virtualization
-  USB Devices 

API Collection

# USB Devices

## Topics

### Storage Devices

class VZUSBMassStorageDevice

A class that represents a hot-pluggable USB mass storage device.

### Configurations

class VZUSBControllerConfiguration

The base class for a USB controller configuration.

class VZXHCIControllerConfiguration

The configuration object for the USB Extensible Host Controller Interface (XHCI) controller.

### Controllers

class VZUSBController

A class that represents a USB controller in a VM.

class VZXHCIController

A class that represents a USB Extensible Host Controller Interface (XHCI) controller in a VM.

### Protocols

protocol VZUSBDevice

A protocol that represents a USB device in a VM.

protocol VZUSBDeviceConfiguration

The protocol for configuring USB devices.

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

Sockets

Configure a device that manages port-based communication with the guest system.

Storage

Configure the block-storage devices that represent the disks of the guest system.

Consoles

Configure a device that manages multiport console communication with the guest system.

Clipboard sharing

Share the pasteboard between the host and guest system.

