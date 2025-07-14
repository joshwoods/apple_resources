

- Core Media
-  CMTimeMapping APIs 

API Collection

# CMTimeMapping APIs

A structure that maps a segment of a source time range to a target time range.

## Topics

### Creating Time Mappings

func CMTimeMappingMake(source: CMTimeRange, target: CMTimeRange) -> CMTimeMapping

Creates a time mapping with a source and target time range.

func CMTimeMappingMakeEmpty(target: CMTimeRange) -> CMTimeMapping

Creates a valid time mapping with an empty source.

func CMTimeMappingMakeFromDictionary(CFDictionary) -> CMTimeMapping

Creates a time mapping from a dictionary representation.

### Representing Time Mappings

func CMTimeMappingCopyAsDictionary(CMTimeMapping, allocator: CFAllocator?) -> CFDictionary?

Returns a dictionary representation of a time mapping.

func CMTimeMappingCopyDescription(allocator: CFAllocator?, mapping: CMTimeMapping) -> CFString?

Copies a string description of a time mapping.

func CMTimeMappingShow(CMTimeMapping)

Prints a description of a time mapping to standard output.

### Data Types

struct CMTimeMapping

A structure that maps a segment of a source time range to a target time range.

### Constants

static let invalid: CMTimeMapping

An invalid time mapping.

let kCMTimeMappingSourceKey: CFString

A dictionary key for a source time range.

let kCMTimeMappingTargetKey: CFString

A dictionary key for a target time range.

## See Also

### Time Representation

CMTime APIs

A structure that represents time.

CMTimeRange APIs

A structure that represents a range of time.

