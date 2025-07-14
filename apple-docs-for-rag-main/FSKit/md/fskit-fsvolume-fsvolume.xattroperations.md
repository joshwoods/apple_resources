

- FSKit
- FSVolume
-  FSVolume.XattrOperations 

Protocol

# FSVolume.XattrOperations

Methods and properties implemented by volumes that natively or partially support extended attributes.

macOS 15.4+

``` source
protocol XattrOperations : NSObjectProtocol
```

## Topics

### Reading and writing

func getXattr(named: FSFileName, of: FSItem, replyHandler: (Data?, (any Error)?) -> Void)

Gets the specified extended attribute of the given item.

**Required**

func listXattrs(of: FSItem, replyHandler: ([FSFileName]?, (any Error)?) -> Void)

Gets the list of extended attributes currently set on the given item.

**Required**

func setXattr(named: FSFileName, to: Data?, on: FSItem, policy: FSVolume.SetXattrPolicy, replyHandler: ((any Error)?) -> Void)

Sets the specified extended attribute data on the given item.

**Required**

enum SetXattrPolicy

Flags to specify the policy when setting extended file attributes.

func supportedXattrNames(for: FSItem) -> [FSFileName]

Returns an array that specifies the extended attribute names the given item supports.

### Inspecting volume properties

var xattrOperationsInhibited: Bool

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

protocol AccessCheckOperations

Methods and properties implemented by volumes that want to enforce access check operations.

protocol RenameOperations

Methods and properties implemented by volumes that support renaming the volume.

protocol FSVolumeKernelOffloadedIOOperations

Methods and properties implemented by volumes that use kernel-offloaded I/O to achieve higher file transfer performance.

protocol PreallocateOperations

Methods and properties implemented by volumes that want to offer preallocation functions.

protocol ItemDeactivation

Methods and properties implemented by volumes that support deactivating items.

