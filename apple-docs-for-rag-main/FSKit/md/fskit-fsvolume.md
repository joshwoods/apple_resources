

- FSKit
-  FSVolume 

Class

# FSVolume

A directory structure for files and folders.

macOS 15.4+

``` source
class FSVolume
```

## Overview

A file system, depending on its type, provides one or more volumes to clients. The FSUnaryFileSystem by definition provides only one volume, while an FSFileSystem supports multiple volumes.

You implement a volume for your file system type by subclassing this class, and also conforming to the FSVolume.Operations and FSVolume.PathConfOperations protocols. This protocol defines the minimum set of operations supported by a volume, such as mounting, activating, creating and removing items, and more.

Your volume can provide additional functionality by conforming to other volume operations protocols. These protocols add support for operations like open and close, read and write, extended attribute (Xattr) manipulation, and more.

## Topics

### Creating a volume

init(volumeID: FSVolume.Identifier, volumeName: FSFileName)

Creates a volume with the given identifier and name.

class Identifier

A type that identifies a volume.

class FSFileName

The name of a file, expressed as a data buffer.

### Accessing volume properties

var volumeID: FSVolume.Identifier

An identifier that uniquely identifies the volume.

var name: FSFileName

The name of the volume.

### Implementing required operations

protocol Operations

Methods that all volumes implement to provide required capabilities.

protocol PathConfOperations

Properties implemented by volumes that support providing the values of system limits or options.

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

protocol ItemDeactivation

Methods and properties implemented by volumes that support deactivating items.

### Default Implementations

Identifiable Implementations

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- NSObjectProtocol

