

- Core Services
- File System Events
-  FSEventStreamScheduleWithRunLoop(\_:\_:\_:) Deprecated

Function

# FSEventStreamScheduleWithRunLoop(\_:\_:\_:)

Mac Catalyst 13.1–16.0DeprecatedmacOS 10.5–13.0Deprecated

``` source
func FSEventStreamScheduleWithRunLoop(
    _ streamRef: FSEventStreamRef,
    _ runLoop: CFRunLoop,
    _ runLoopMode: CFString
)
```

Deprecated

Use FSEventStreamSetDispatchQueue(_:_:) instead.

## Parameters 

`streamRef`  

A valid stream.

`runLoop`  

The run loop on which to schedule the stream.

`runLoopMode`  

A run loop mode on which to schedule the stream.

## Discussion

This function schedules the stream on the specified run loop, like CFRunLoopAddSource() does for a CFRunLoopSourceRef. The caller is responsible for ensuring that the stream is scheduled on at least one run loop and that at least one of the run loops on which the stream is scheduled is being run.

To start receiving events on the stream, call FSEventStreamStart().

To remove the stream from the run loops upon which it has been scheduled, call FSEventStreamUnscheduleFromRunLoop() or FSEventStreamInvalidate().

