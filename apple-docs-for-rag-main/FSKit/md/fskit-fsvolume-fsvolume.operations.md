

- FSKit
- FSVolume
-  FSVolume.Operations 

Protocol

# FSVolume.Operations

Methods that all volumes implement to provide required capabilities.

macOS 15.4+

``` source
protocol Operations : FSVolume.PathConfOperations
```

## Overview

Conform to this protocol in your subclass of FSVolume. To provide additional capabilities, conform to the other `FSVolume` operations protocols, like FSVolume.OpenCloseOperations and FSVolume.ReadWriteOperations.

Note

This protocol extends FSVolume.PathConfOperations, so your volume implementation must also conform to that protocol.

## Topics

### Handling activation and deactivation

func activate(options: FSTaskOptions, replyHandler: (FSItem?, (any Error)?) -> Void)

Activates the volume using the specified options.

**Required**

class FSItem

A distinct object in a file hierarchy, such as a file, directory, symlink, socket, and more.

func deactivate(options: FSDeactivateOptions, replyHandler: ((any Error)?) -> Void)

Tears down a previously initialized volume instance.

**Required**

struct FSDeactivateOptions

Options that affect the behavior of deactivate methods.

### Mounting and unmounting

func mount(options: FSTaskOptions, replyHandler: ((any Error)?) -> Void)

Mounts this volume, using the specified options.

**Required**

func unmount(replyHandler: () -> Void)

Unmounts this volume.

**Required**

### Working with items

func createItem(named: FSFileName, type: FSItem.ItemType, inDirectory: FSItem, attributes: FSItem.SetAttributesRequest, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Creates a new file or directory item.

**Required**

class FSFileName

The name of a file, expressed as a data buffer.

enum ItemType

An enumeration of item types, such as file, directory, or symbolic link.

class SetAttributesRequest

A request to set attributes on an item.

func lookupItem(named: FSFileName, inDirectory: FSItem, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Looks up an item within a directory.

**Required**

func removeItem(FSItem, named: FSFileName, fromDirectory: FSItem, replyHandler: ((any Error)?) -> Void)

Removes an existing item from a given directory.

**Required**

func renameItem(FSItem, inDirectory: FSItem, named: FSFileName, to: FSFileName, inDirectory: FSItem, overItem: FSItem?, replyHandler: (FSFileName?, (any Error)?) -> Void)

Renames an item from one path in the file system to another.

**Required**

func reclaimItem(FSItem, replyHandler: ((any Error)?) -> Void)

Reclaims an item, releasing any resources allocated for the item.

**Required**

### Working with links

func createLink(to: FSItem, named: FSFileName, inDirectory: FSItem, replyHandler: (FSFileName?, (any Error)?) -> Void)

Creates a new hard link.

**Required**

func createSymbolicLink(named: FSFileName, inDirectory: FSItem, attributes: FSItem.SetAttributesRequest, linkContents: FSFileName, replyHandler: (FSItem?, FSFileName?, (any Error)?) -> Void)

Creates a new symbolic link.

**Required**

func readSymbolicLink(FSItem, replyHandler: (FSFileName?, (any Error)?) -> Void)

Reads a symbolic link.

**Required**

### Working with attributes

func getAttributes(FSItem.GetAttributesRequest, of: FSItem, replyHandler: (FSItem.Attributes?, (any Error)?) -> Void)

Fetches attributes for the given item.

**Required**

class GetAttributesRequest

A request to get attributes from an item.

func setAttributes(FSItem.SetAttributesRequest, on: FSItem, replyHandler: (FSItem.Attributes?, (any Error)?) -> Void)

Sets the given attributes on an item.

**Required**

class SetAttributesRequest

A request to set attributes on an item.

### Inspecting directory contents

func enumerateDirectory(FSItem, startingAt: FSDirectoryCookie, verifier: FSDirectoryVerifier, attributes: FSItem.GetAttributesRequest?, packer: FSDirectoryEntryPacker, replyHandler: (FSDirectoryVerifier, (any Error)?) -> Void)

Enumerates the contents of the given directory.

**Required**

struct FSDirectoryCookie

A value that indicates a location in a directory from which to enumerate.

struct FSDirectoryCookie

A value that indicates a location in a directory from which to enumerate.

struct FSDirectoryVerifier

A tool to detect whether the directory contents changed since the last call to enumerate a directory.

struct FSDirectoryVerifier

A tool to detect whether the directory contents changed since the last call to enumerate a directory.

class FSDirectoryEntryPacker

An object used to provide items during a directory enumeration.

### Synchronizing with a resource

func synchronize(flags: FSSyncFlags, replyHandler: ((any Error)?) -> Void)

Synchronizes the volume with its underlying resource.

**Required**

enum FSSyncFlags

Behavior flags for use with synchronization calls.

### Inspecting volume properties

var supportedVolumeCapabilities: FSVolume.SupportedCapabilities

A property that provides the supported capabilities of the volume.

**Required**

class SupportedCapabilities

A type that represents capabillities supported by a volume, such as hard and symbolic links, journaling, and large file sizes.

var volumeStatistics: FSStatFSResult

A property that provides up-to-date statistics of the volume.

**Required**

class FSStatFSResult

A type used to report a volume’s statistics.

## Relationships

### Inherits From

- FSVolume.PathConfOperations
- NSObjectProtocol

## See Also

### Implementing required operations

protocol PathConfOperations

Properties implemented by volumes that support providing the values of system limits or options.

