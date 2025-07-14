

- os
-  os_signpost(\_:dso:log:name:signpostID:\_:\_:) Deprecated

Function

# os_signpost(\_:dso:log:name:signpostID:\_:\_:)

Logs a point of interest in your code as a time interval or as an event for debugging performance in Instruments, and includes a detailed message.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOSwatchOS 5.0+

``` source
func os_signpost(
    _ type: OSSignpostType,
    dso: UnsafeRawPointer = #dsohandle,
    log: OSLog,
    name: StaticString,
    signpostID: OSSignpostID = .exclusive,
    _ format: StaticString,
    _ arguments: any CVarArg...
)
```

Deprecated

Use beginInterval(_:id:_:) instead.

## Parameters 

`type`  

The type of signpost to log.

`log`  

A log object to log the signpost to.

`name`  

The name of the signpost.

`signpostID`  

A signpost identifier you use to disambiguate between signposts with the same name.

`format`  

A constant string or format string that produces a human-readable log message.

`arguments`  

Additional arguments to substitute into the `format` string parameter. Pass the expected number of arguments in the order that they appear in the string. If `format` is a constant string, don’t include any additional arguments.

## See Also

### Measure Events

func os_signpost(OSSignpostType, dso: UnsafeRawPointer, log: OSLog, name: StaticString, signpostID: OSSignpostID)

Logs a point of interest in your code as a time interval or as an event for debugging performance in Instruments.

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

