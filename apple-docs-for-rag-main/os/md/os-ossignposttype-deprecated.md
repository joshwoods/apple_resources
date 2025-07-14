

- os
-  OSSignpostType Deprecated

Structure

# OSSignpostType

The different kinds of signpost.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct OSSignpostType
```

Deprecated

Use OSSignposter instead.

## Topics

### Specifying Signpost Types

static let begin: OSSignpostType

A signpost that marks the start of a time interval of interest in your code.

static let end: OSSignpostType

A signpost that marks the end of a time interval of interest in your code.

static let event: OSSignpostType

A signpost that marks an event in your code.

### Creating Signpost Types

init(rawValue: UInt8)

Creates a signpost from a raw integer value.

init(UInt8)

Creates a signpost from a raw integer value.

### Inspecting Signpost Types

var rawValue: UInt8

An integer value that represents the role of a signpost.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Measure Events

Recording Performance Data

Add signposts to record interesting time-based events.

struct OSSignposter

An object for measuring task performance using the unified logging system.

Legacy Signpost Symbols

Migrate your code away from using these legacy symbols.

typealias os_signpost_id_t

An identifier you use to distinguish between signposts that have the same name and destination log.

