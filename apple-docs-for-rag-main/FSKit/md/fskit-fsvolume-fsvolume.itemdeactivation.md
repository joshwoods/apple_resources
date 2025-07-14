

- FSKit
- FSVolume
-  FSVolume.ItemDeactivation 

Protocol

# FSVolume.ItemDeactivation

Methods and properties implemented by volumes that support deactivating items.

macOS 15.4+

``` source
protocol ItemDeactivation : NSObjectProtocol
```

## Topics

### Deactivating an item

func deactivateItem(FSItem, replyHandler: ((any Error)?) -> Void)

Notifies the file system that the kernel is no longer making immediate use of the given item.

**Required**

### Setting deactivation policy

var itemDeactivationPolicy: FSVolume.ItemDeactivationOptions

A property that tells FSKit to which types of items the deactivation applies, if any.

**Required**

struct ItemDeactivationOptions

Options to specify the item deactivation policy.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Implementing optional operations

protocol OpenCloseOperations

Methods and properties implemented by volumes that want to receive open and close calls for each item.

protocol ReadWriteOperations

Methods implemented for read and write operations that deliver data to and from the extension.

protocol AccessCheckOperations

Methods and properties implemented by volumes that want to enforce access check operations.

protocol RenameOperations

Methods and properties implemented by volumes that support renaming the volume.

protocol FSVolumeKernelOffloadedIOOperations

Methods and properties implemented by volumes that use kernel-offloaded I/O to achieve higher file transfer performance.

protocol PreallocateOperations

Methods and properties implemented by volumes that want to offer preallocation functions.

protocol XattrOperations

Methods and properties implemented by volumes that natively or partially support extended attributes.

