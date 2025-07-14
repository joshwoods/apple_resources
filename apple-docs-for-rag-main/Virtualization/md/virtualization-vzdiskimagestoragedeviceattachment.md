

- Virtualization
-  VZDiskImageStorageDeviceAttachment 

Class

# VZDiskImageStorageDeviceAttachment

A device that stores content in a disk image.

macOS 11.0+

``` source
class VZDiskImageStorageDeviceAttachment
```

## Overview

Use a VZDiskImageStorageDeviceAttachment object to manage the storage for a disk in the virtual machine. The guest operating system sees the storage as a disk. When the guest operating system writes files to disk, the virtual machine stores those files in the disk image you provide.

Create a RAW disk image in the file system of the host computer, and use that disk image to initialize your VZDiskImageStorageDeviceAttachment object. Use the attachment object to configure the VZVirtioBlockDeviceConfiguration object that you add to your virtual machine’s configuration.

## Topics

### Creating the attachment point

init(url: URL, readOnly: Bool) throws

Creates the attachment object from the specified disk image.

init(url: URL, readOnly: Bool, cachingMode: VZDiskImageCachingMode, synchronizationMode: VZDiskImageSynchronizationMode) throws

Initialize the attachment from a local file URL.

### Getting the disk image details

var url: URL

The URL of the underlying disk image.

var isReadOnly: Bool

A Boolean value that indicates whether the underlying disk image is read-only.

var cachingMode: VZDiskImageCachingMode

The current cacheing mode for the virtual disk image.

var synchronizationMode: VZDiskImageSynchronizationMode

The mode in which the disk image synchronizes data with the underlying storage device.

## Relationships

### Inherits From

- VZStorageDeviceAttachment

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Attachment points

class VZDiskBlockDeviceStorageDeviceAttachment

A storage device attachment that uses a disk to store data.

class VZNetworkBlockDeviceStorageDeviceAttachment

A storage device attachment backed by a Network Block Device (NBD) client.

class VZStorageDeviceAttachment

The common behaviors for storage devices in the guest system.

