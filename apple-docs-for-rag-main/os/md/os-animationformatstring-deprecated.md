

- os
-  AnimationFormatString Deprecated

Enumeration

# AnimationFormatString

A namespace for utilities specific to animation-related signposts.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum AnimationFormatString
```

Deprecated

Use OSSignposter instead.

## Topics

### Getting an Animation-Related Log Message

struct OSLogMessage

A log message that includes an animation tag.

## See Also

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

typealias os_signpost_id_t

An identifier you use to distinguish between signposts that have the same name and destination log.

