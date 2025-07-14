

- FSKit
-  FSExtentType 

Enumeration

# FSExtentType

An enumeration of types of extents.

macOS 15.4+

``` source
enum FSExtentType
```

## Topics

### Working with extent types

case data

An extent type to indicate valid data.

case zeroFill

An extent type to indicate uninitialized data.

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

enum FSMatchResult

A type that represents the recognition and usability of a probed resource.

class FSMetadataRange

A range that describes contiguous metadata segments on disk.

class FSProbeResult

An object that represents the results of a specific probe.

