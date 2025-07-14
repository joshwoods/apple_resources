

- Virtualization
-  Storage 

API Collection

# Storage

Configure the block-storage devices that represent the disks of the guest system.

## Topics

### Configurations

class VZVirtioBlockDeviceConfiguration

The configuration object that requests the creation of a virtual storage device in the guest system.

class VZStorageDeviceConfiguration

The common configuration traits for storage device requests.

class VZUSBMassStorageDeviceConfiguration

The configuration object that represents a USB Mass storage device.

enum VZDiskImageCachingMode

An integer that describes the disk image caching mode.

enum VZDiskImageSynchronizationMode

An integer that describes the disk image synchronization mode.

class VZNVMExpressControllerDeviceConfiguration

The configuration object that represents an NVM Express Controller storage device.

### Devices

class VZStorageDevice

A class that represents a storage device in a VM.

### Attachment points

class VZDiskBlockDeviceStorageDeviceAttachment

A storage device attachment that uses a disk to store data.

class VZDiskImageStorageDeviceAttachment

A device that stores content in a disk image.

class VZNetworkBlockDeviceStorageDeviceAttachment

A storage device attachment backed by a Network Block Device (NBD) client.

class VZStorageDeviceAttachment

The common behaviors for storage devices in the guest system.

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

Consoles

Configure a device that manages multiport console communication with the guest system.

Clipboard sharing

Share the pasteboard between the host and guest system.

USB Devices

