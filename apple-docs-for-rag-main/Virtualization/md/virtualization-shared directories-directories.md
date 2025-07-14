

- Virtualization
-  Shared directories 

API Collection

# Shared directories

Configure devices that share directories from the host into the guest system.

## Overview

Shared directories allow you expose specific directories in the macOS file system to the guest operating system running in a VM, this allows your user to share files between the host and guest operating system. To enable shared directory device support in Linux, configure the Linux guest kernel to enable the `CONFIG_VIRTIO_FS` support.

Configure a VIRTIO file system device using a VZVirtioFileSystemDeviceConfiguration. The guest can use the tag label to mount and access the host resources.

The VZDirectoryShare on the configuration defines the host directories to expose to the guest. To limit or expose new directories to the guest while the VM is running, you can update the directory share with VZVirtioFileSystemDevice.

Use VZSingleDirectoryShare to share the immediate contents of a single directory on the host, or use VZMultipleDirectoryShare to share multiple directories from the host and include a specific name for each shared directory.

Note

Shared directories in macOS VMs are only available in macOS 13 and later.

## Topics

### Configurations

class VZVirtioFileSystemDeviceConfiguration

An object that represents the configuration of a Virtio file system device.

class VZDirectorySharingDeviceConfiguration

The base class for a directory sharing device configuration.

class VZLinuxRosettaDirectoryShare

The Linux directory share for Rosetta.

### Shared directory devices

class VZVirtioFileSystemDevice

An object the defines a VIRTIO file system device.

class VZDirectorySharingDevice

The base class that represents a directory sharing device in a VM.

### Directory Shares

class VZMultipleDirectoryShare

An object that describes a directory share for multiple directories.

class VZSingleDirectoryShare

An object that defines the directory share for a single directory.

class VZSharedDirectory

A directory on the host that you can expose to a guest.

class VZDirectoryShare

The base class for a directory share.

class VZLinuxRosettaDirectoryShare

The Linux directory share for Rosetta.

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

Sockets

Configure a device that manages port-based communication with the guest system.

Storage

Configure the block-storage devices that represent the disks of the guest system.

Consoles

Configure a device that manages multiport console communication with the guest system.

Clipboard sharing

Share the pasteboard between the host and guest system.

USB Devices

