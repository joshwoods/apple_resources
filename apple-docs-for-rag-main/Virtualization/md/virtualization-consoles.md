

- Virtualization
-  Consoles 

API Collection

# Consoles

Configure a device that manages multiport console communication with the guest system.

## Topics

### Configurations

class VZConsoleDeviceConfiguration

The base class for a console device configuration.

class VZConsolePortConfiguration

The base class for a console port configuration.

class VZVirtioConsoleDeviceConfiguration

A console device that enables communication between the host and the guest using console ports through a Virtio interface.

class VZVirtioConsolePortConfiguration

A class that represents the configuration options you can set on a Virtio console port.

class VZVirtioConsolePortConfigurationArray

A class that represents a collection of Virtio console port configurations.

### Console ports

class VZVirtioConsolePort

A class that represents a Virtio console port in a VM.

class VZVirtioConsolePortArray

A class that represents a collection of Virtio console ports.

### Devices

class VZConsoleDevice

A class that represents a console device in a VM.

class VZVirtioConsoleDevice

A class that represents a Virtio console device in a virtual machine.

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

Clipboard sharing

Share the pasteboard between the host and guest system.

USB Devices

