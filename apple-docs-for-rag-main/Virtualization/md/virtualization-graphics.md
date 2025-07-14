

- Virtualization
-  Graphics 

API Collection

# Graphics

Configure a device for a guest to display its UI.

## Overview

A graphics devices allows people to see and interact with the UI of a VM, you use this device to attach a display that’s shown in a VZVirtualMachineView.

## Topics

### Configurations

class VZGraphicsDisplayConfiguration

The base class for a graphics display configuration.

class VZMacGraphicsDeviceConfiguration

Configuration for a display attached to a Mac graphics device.

class VZMacGraphicsDisplayConfiguration

The configuration for a Mac graphics device.

class VZGraphicsDeviceConfiguration

The base class for a graphics device configuration.

class VZVirtioGraphicsDeviceConfiguration

Configuration that represents the configuration of a Virtio graphics device for a Linux VM.

### Devices

class VZGraphicsDevice

A class that represents a graphics device in a VM.

class VZGraphicsDisplay

A class that represents a graphics display in a VM.

class VZMacGraphicsDevice

An object that represents a Mac graphics device.

class VZVirtioGraphicsScanout

A Virtio graphics scanout that corresponds to a Virtio graphics scanout configuration.

class VZMacGraphicsDisplay

An object that represents the graphics display on a Mac.

class VZVirtioGraphicsDevice

A Virtio graphics device.

## See Also

### Devices

Audio

Configure audio devices that enable the guest operating system to perform audio playback and capture through the host’s audio devices.

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

USB Devices

