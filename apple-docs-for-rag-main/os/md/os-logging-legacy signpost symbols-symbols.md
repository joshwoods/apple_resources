

- os
- Logging
-  Legacy Signpost Symbols 

API Collection

# Legacy Signpost Symbols

Migrate your code away from using these legacy symbols.

## Topics

### Measure Events

func os_signpost(OSSignpostType, dso: UnsafeRawPointer, log: OSLog, name: StaticString, signpostID: OSSignpostID)

Logs a point of interest in your code as a time interval or as an event for debugging performance in Instruments.

Deprecated

func os_signpost(OSSignpostType, dso: UnsafeRawPointer, log: OSLog, name: StaticString, signpostID: OSSignpostID, StaticString, any CVarArg...)

Logs a point of interest in your code as a time interval or as an event for debugging performance in Instruments, and includes a detailed message.

Deprecated

struct OSSignpostType

The different kinds of signpost.

Deprecated

func os_signpost(OSSignpostAnimationBegin, dso: UnsafeRawPointer, log: OSLog, name: StaticString, signpostID: OSSignpostID)

Logs the beginning of an animation as a point-of-interest in your code, without a message.

Deprecated

func os_signpost(OSSignpostAnimationBegin, dso: UnsafeRawPointer, log: OSLog, name: StaticString, signpostID: OSSignpostID, AnimationFormatString.OSLogMessage, any CVarArg...)

Logs the beginning of an animation as a point-of-interest in your code, and includes the specified message in the logs.

Deprecated

enum OSSignpostAnimationBegin

The signpost options to use when measuring animations.

Deprecated

enum AnimationFormatString

A namespace for utilities specific to animation-related signposts.

Deprecated

typealias os_signpost_id_t

An identifier you use to distinguish between signposts that have the same name and destination log.

## See Also

### Measure Events

Recording Performance Data

Add signposts to record interesting time-based events.

struct OSSignposter

An object for measuring task performance using the unified logging system.

struct OSSignpostType

The different kinds of signpost.

Deprecated

typealias os_signpost_id_t

An identifier you use to distinguish between signposts that have the same name and destination log.

