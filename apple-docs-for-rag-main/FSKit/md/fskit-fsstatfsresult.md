

- FSKit
-  FSStatFSResult 

Class

# FSStatFSResult

A type used to report a volume’s statistics.

macOS 15.4+

``` source
class FSStatFSResult
```

## Overview

The names of this type’s properties match those in the `statfs` structure in `statfs(2)`, which reports these values for an FSKit file system. All numeric properties default to `0`. Override these values, unless a given property has no meaningful value to provide.

Note

Available space, free space, total space, and used space have properties to express their values either as a number of blocks or a number of bytes. Your module may supply both of these values by setting both the relevant block or byte property. Alternatively, a module may set only one of the two properties. When you do this, FSKit calculates the matching value based on blockSize.

For the read-only fileSystemTypeName, set this value with the designated initializer.

## Topics

### Initializers

init(fileSystemTypeName: String)

Creates an statistics result instance, using the given file system type name.

### Instance Properties

var availableBlocks: UInt64

A property for the number of free blocks available to a non-superuser on the volume.

var availableBytes: UInt64

A property for the amount of space available to users, in bytes, in the volume.

var blockSize: Int

A property for the volume’s block size, in bytes.

var fileSystemSubType: Int

A property for the file system’s subtype or flavor.

var fileSystemTypeName: String

A property for the file system type name.

var freeBlocks: UInt64

A property for the number of free blocks in the volume.

var freeBytes: UInt64

A property for the amount of free space, in bytes, in the volume.

var freeFiles: UInt64

A property for the total number of free file slots in the volume.

var ioSize: Int

A property for the optimal block size with which to perform I/O.

var totalBlocks: UInt64

A property for the volume’s total data block count.

var totalBytes: UInt64

A property for the total size, in bytes, of the volume.

var totalFiles: UInt64

A property for the total number of file slots in the volume,

var usedBlocks: UInt64

A property for the number of used blocks in the volume.

var usedBytes: UInt64

A property for the amount of used space, in bytes, in the volume.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Inspecting volume properties

var supportedVolumeCapabilities: FSVolume.SupportedCapabilities

A property that provides the supported capabilities of the volume.

**Required**

class SupportedCapabilities

A type that represents capabillities supported by a volume, such as hard and symbolic links, journaling, and large file sizes.

var volumeStatistics: FSStatFSResult

A property that provides up-to-date statistics of the volume.

**Required**

