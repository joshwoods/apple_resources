

- Virtualization
-  VZVirtioFileSystemDevice 

Class

# VZVirtioFileSystemDevice

An object the defines a VIRTIO file system device.

macOS 12.0+

``` source
class VZVirtioFileSystemDevice
```

## Overview

This device exposes host resources to the guest as a file system mount. The directory share defines which resources the host exposes to the guest.

Create this device by instantiating a VZVirtioFileSystemDeviceConfiguration in a VZVirtualMachineConfiguration. The file system device is available in the `VZVirtualMachine`.directorySharingDevices property. The guest can use the tag label to mount and access the host resources.

With `VZVirtioFileSystemDevice`, the framework enforces several permissions policies for shared directories:

- The framework reads and writes files using the user ID (UID) of the effective user, which is the UID of the current user, rather than the UID of the system process.

- The framework doesn’t allow reading or overwriting of files with permissions where the file is inaccessible to the current user.

- The framework ignores requests from guest operating systems to change the UID or group ID (GID) of files on the host.

## Topics

### Accessing directory properties

var share: VZDirectoryShare?

A value that defines the directory share the host exposes to the guest VM.

var tag: String

A string that identifies the device.

## Relationships

### Inherits From

- VZDirectorySharingDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZVirtioFileSystemDeviceConfiguration

An object that represents the configuration of a Virtio file system device.

class VZSingleDirectoryShare

An object that defines the directory share for a single directory.

class VZMultipleDirectoryShare

An object that describes a directory share for multiple directories.

### Shared directory devices

class VZDirectorySharingDevice

The base class that represents a directory sharing device in a VM.

