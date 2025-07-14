

- FSKit
-  FSProbeResult 

Class

# FSProbeResult

An object that represents the results of a specific probe.

macOS 15.4+

``` source
class FSProbeResult
```

## Overview

For any result value other than FSMatchResult.notRecognized, ensure the name and containerID values are non-`nil`. When a container or volume format doesn’t use a name, return an empty string. Also use an empty string in the case in which the format supports a name, but the value isn’t set yet.

Some container or volume formats may lack a durable UUID on which to base a container identifier. This situation is only valid for unary file systems. In such a case, return a random UUID.

With a block device resource, a probe operation may successfully get a result but encounter an error reading the name or UUID. If this happens, use whatever information is available, and provide an empty string or random UUID for the name or container ID, respectively.

## Topics

### Working with results

class func recognized(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized file system.

class func usable(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized and usable file system.

class func usableButLimited(name: String, containerID: FSContainerIdentifier) -> Self

Creates a probe result for a recognized file system that is usable, but with limited capabilities.

class var usableButLimited: FSProbeResult

A probe result for a recognized file system that is usable, but with limited capabilities.

class var notRecognized: FSProbeResult

A probe result for an unrecognized file system.

### Working with result properties

var containerID: FSContainerIdentifier?

The container identifier, as found during the probe operation.

var name: String?

The resource name, as found during the probe operation.

var result: FSMatchResult

The match result, representing the recognition and usability of a probed resource.

enum FSMatchResult

A type that represents the recognition and usability of a probed resource.

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

enum FSMatchResult

A type that represents the recognition and usability of a probed resource.

class FSMetadataRange

A range that describes contiguous metadata segments on disk.

