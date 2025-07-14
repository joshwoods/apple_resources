

- FSKit
-  FSMatchResult 

Enumeration

# FSMatchResult

A type that represents the recognition and usability of a probed resource.

macOS 15.4+

``` source
enum FSMatchResult
```

## Topics

### Working with match results

case usable

The probe recognizes the resource and is ready to use it.

case usableButLimited

The probe recognizes the resource and is ready to use it, but only in a limited capacity.

case recognized

The probe recognizes the resource but can’t use it.

case notRecognized

The probe doesn’t recognize the resource.

### Working with raw values

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting types

struct FSBlockmapFlags

Flags that describe the behavior of a blockmap operation.

struct FSCompleteIOFlags

Flags that describe the behavior of an I/O completion operation.

class FSEntityIdentifier

A base type that identifies containers and volumes.

class FSExtentPacker

A type that directs the kernel to map space on disk to a specific file managed by this file system.

enum FSExtentType

An enumeration of types of extents.

class FSMetadataRange

A range that describes contiguous metadata segments on disk.

class FSProbeResult

An object that represents the results of a specific probe.

