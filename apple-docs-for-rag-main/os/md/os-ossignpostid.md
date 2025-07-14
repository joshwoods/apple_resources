

- os
-  OSSignpostID 

Structure

# OSSignpostID

An identifier that disambiguates signposted intervals.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOSwatchOS 5.0+

``` source
struct OSSignpostID
```

## Mentioned in 

Recording Performance Data

## Overview

Multiple intervals that have matching names, subsystems, and categories, and that exist in the same scope can be in-flight simultaneously. To match a pair of interval calls, you need to identify each interval with a unique signpost identifier. Use the first strategy in the list below that matches your use case:

- If identical intervals can never overlap, use the exclusive signpost ID.

- If you have data that uniquely identifies each instance of the measured task, create a signpost ID using the init(_:) method. The value you provide must not match that of any of the system-defined signpost IDs.

- If you have an object that uniquely identifies a pair of interval calls, such as the object you’re measuring, create a signpost ID using the makeSignpostID(from:) method. Don’t use this method for signposts that cross process boundaries.

- Otherwise, create a signpost ID using the makeSignpostID() method.

## Topics

### Getting Signpost Identifiers

static let exclusive: OSSignpostID

A signpost identifier that indicates no overlap among different signpost time intervals.

static let invalid: OSSignpostID

A signpost identifier that indicates an error.

static let null: OSSignpostID

A signpost identifier that indicates a disabled signpost.

### Creating a Signpost Identifier

init(UInt64)

Creates a signpost ID from an arbitrary 64-bit integer value.

init(log: OSLog)

Creates a signpost ID for the specified log.

Deprecated

init(log: OSLog, object: AnyObject)

Creates a signpost ID and associates it with the specified object.

Deprecated

### Getting an Identifier’s Raw Value

let rawValue: os_signpost_id_t

The signpost ID’s raw value.

## Relationships

### Conforms To

- Comparable
- Copyable
- Equatable
- Sendable

## See Also

### Generating Signpost IDs

func makeSignpostID() -> OSSignpostID

Returns an identifier that’s unique within the scope of the signposter.

func makeSignpostID(from: AnyObject) -> OSSignpostID

Returns an identifier that the signposter derives from the specified object.

