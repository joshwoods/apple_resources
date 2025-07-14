

- FSKit
- FSVolume
-  FSVolume.PathConfOperations 

Protocol

# FSVolume.PathConfOperations

Properties implemented by volumes that support providing the values of system limits or options.

macOS 15.4+

``` source
protocol PathConfOperations : NSObjectProtocol
```

## Overview

This protocol gathers properties related to the `pathconf` and `fpathconf` system calls.

For a file, the value of a property applies to just that file; for a directory, the value applies to all items in the directory.

Properties that represent limits and have a numeric type use `-1` to represent no limit.

## Topics

### Checking limits and configurations

var maximumLinkCount: Int

A property that represents the maximum number of hard links to the object.

**Required**

var maximumNameLength: Int

A property that represents the maximum length of a component of a filename.

**Required**

var restrictsOwnershipChanges: Bool

A Boolean property that indicates whether the volume restricts ownership changes based on authorization.

**Required**

var truncatesLongNames: Bool

A property that indicates whether the volume truncates files longer than its maximum supported length.

**Required**

var maximumFileSize: UInt64

The maximum size of a regular file allowed in the volume.

var maximumFileSizeInBits: Int

The minimum number of bits needed to represent, as a signed integer value, the maximum size of a regular file allowed in the volume.

var maximumXattrSize: Int

The maximum extended attribute size in bytes.

var maximumXattrSizeInBits: Int

The maximum extended attribute size in bits.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- FSVolume.Operations

## See Also

### Implementing required operations

protocol Operations

Methods that all volumes implement to provide required capabilities.

