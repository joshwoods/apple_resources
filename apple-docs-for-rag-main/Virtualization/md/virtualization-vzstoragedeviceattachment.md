

- Virtualization
-  VZStorageDeviceAttachment 

Class

# VZStorageDeviceAttachment

The common behaviors for storage devices in the guest system.

macOS 11.0+

``` source
class VZStorageDeviceAttachment
```

## Overview

A VZStorageDeviceAttachment object defines the implementation of a storage interface in a virtual machine. You use the attachment object to specify the source of the storage on the host computer.

Don’t create VZStorageDeviceAttachment objects directly. Instead, instantiate an appropriate subclass such as VZDiskImageStorageDeviceAttachment, which provides storage using a disk image.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZDiskBlockDeviceStorageDeviceAttachment
- VZDiskImageStorageDeviceAttachment
- VZNetworkBlockDeviceStorageDeviceAttachment

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

class VZDiskImageStorageDeviceAttachment

A device that stores content in a disk image.

class VZNetworkBlockDeviceStorageDeviceAttachment

A storage device attachment backed by a Network Block Device (NBD) client.

