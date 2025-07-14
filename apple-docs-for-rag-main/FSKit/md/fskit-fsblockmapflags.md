

- FSKit
-  FSBlockmapFlags 

Structure

# FSBlockmapFlags

Flags that describe the behavior of a blockmap operation.

macOS 15.4+

``` source
struct FSBlockmapFlags
```

## Overview

This type is an option set in Swift. In Objective-C, you use the cases of this enumeration to create a bit field.

## Topics

### Declaring block map behaviors

static var read: FSBlockmapFlags

A flag that describes a read operation.

static var write: FSBlockmapFlags

A flag that describes a write operation.

### Working with raw values

init(rawValue: UInt)

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Supporting types

struct FSCompleteIOFlags

Flags that describe the behavior of an I/O completion operation.

class FSEntityIdentifier

A base type that identifies containers and volumes.

class FSExtentPacker

A type that directs the kernel to map space on disk to a specific file managed by this file system.

enum FSExtentType

An enumeration of types of extents.

enum FSMatchResult

A type that represents the recognition and usability of a probed resource.

class FSMetadataRange

A range that describes contiguous metadata segments on disk.

class FSProbeResult

An object that represents the results of a specific probe.

