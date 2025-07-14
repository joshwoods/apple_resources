

- FSKit
- FSVolume
-  FSVolume.AccessCheckOperations 

Protocol

# FSVolume.AccessCheckOperations

Methods and properties implemented by volumes that want to enforce access check operations.

macOS 15.4+

``` source
protocol AccessCheckOperations : NSObjectProtocol
```

## Topics

### Checking access

func checkAccess(to: FSItem, requestedAccess: FSVolume.AccessMask, replyHandler: (Bool, (any Error)?) -> Void)

Checks whether the file system allows access to the given item.

**Required**

struct AccessMask

A bitmask of access rights.

### Inspecting volume properties

var isAccessCheckInhibited: Bool

A Boolean value that instructs FSKit not to call this protocol’s methods, even if the volume conforms to it.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Implementing optional operations

protocol OpenCloseOperations

Methods and properties implemented by volumes that want to receive open and close calls for each item.

protocol ReadWriteOperations

Methods implemented for read and write operations that deliver data to and from the extension.

protocol RenameOperations

Methods and properties implemented by volumes that support renaming the volume.

protocol FSVolumeKernelOffloadedIOOperations

Methods and properties implemented by volumes that use kernel-offloaded I/O to achieve higher file transfer performance.

protocol PreallocateOperations

Methods and properties implemented by volumes that want to offer preallocation functions.

protocol XattrOperations

Methods and properties implemented by volumes that natively or partially support extended attributes.

protocol ItemDeactivation

Methods and properties implemented by volumes that support deactivating items.

