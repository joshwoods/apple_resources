

- FSKit
-  FSEntityIdentifier 

Class

# FSEntityIdentifier

A base type that identifies containers and volumes.

macOS 15.4+

``` source
class FSEntityIdentifier
```

## Overview

An FSEntityIdentifier is a UUID to identify a container or volume, optionally with eight bytes of qualifying (differentiating) data. You use the qualifiers in cases in which a file server can receive multiple connections from the same client, which differ by user credentials. In this case, the identifier for each client is the server’s base UUID, and a unique qualifier that differs by client.

Important

Don’t subclass this class.

## Topics

### Creating an entity identifier

init()

Creates an entity identifier with a random UUID.

init(uuid: UUID)

Creates an entity identifier with the given UUID.

init(uuid: UUID, data: Data)

Creates an entity identifier with the given UUID and qualifier data.

init(uuid: UUID, qualifier: UInt64)

Creates an entity identifier with the given UUID and qualifier data as a 64-bit unsigned integer.

### Inspecting identifier properties

var uuid: UUID

A UUID to uniquely identify this entity.

var qualifier: Data?

An optional piece of data to distinguish entities that otherwise share the same UUID.

### Default Implementations

Identifiable Implementations

## Relationships

### Inherits From

- NSObject

### Inherited By

- FSContainerIdentifier
- FSVolume.Identifier

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Supporting types

struct FSBlockmapFlags

Flags that describe the behavior of a blockmap operation.

struct FSCompleteIOFlags

Flags that describe the behavior of an I/O completion operation.

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

