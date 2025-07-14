

- Core Services
- File System Events
-  FSEventStreamUnscheduleFromRunLoop(\_:\_:\_:) Deprecated

Function

# FSEventStreamUnscheduleFromRunLoop(\_:\_:\_:)

Mac Catalyst 13.1–16.0DeprecatedmacOS 10.5–13.0Deprecated

``` source
func FSEventStreamUnscheduleFromRunLoop(
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

The run loop from which to unschedule the stream.

`runLoopMode`  

The run loop mode from which to unschedule the stream.

## Discussion

This function removes the stream from the specified run loop, like CFRunLoopRemoveSource() does for a CFRunLoopSourceRef.

