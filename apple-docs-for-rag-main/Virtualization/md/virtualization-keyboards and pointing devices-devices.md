

- Virtualization
-  Keyboards and pointing devices 

API Collection

# Keyboards and pointing devices

Configure devices that connect a mouse and keyboard to the guest system.

## Overview

Configure a keyboard and a pointing device to allow people to interact with macOS or Linux VMs.

## Topics

### Keyboards

class VZKeyboardConfiguration

The base class for a configuring a keyboard.

class VZMacKeyboardConfiguration

A device that defines the configuration for a Mac keyboard.

class VZUSBKeyboardConfiguration

A device that defines the configuration for a USB keyboard.

### Pointing devices

class VZMacTrackpadConfiguration

The class that represents the configuration for a Mac trackpad.

class VZUSBScreenCoordinatePointingDeviceConfiguration

An object that defines the configuration for a USB pointing device that reports absolute coordinates.

class VZPointingDeviceConfiguration

The base class for a pointing device configuration.

## See Also

### Devices

Audio

Configure audio devices that enable the guest operating system to perform audio playback and capture through the host’s audio devices.

Graphics

Configure a device for a guest to display its UI.

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

