

- Core Services
- File System Events
-  FSEventStreamInvalidate(\_:) 

Function

# FSEventStreamInvalidate(\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func FSEventStreamInvalidate(_ streamRef: FSEventStreamRef)
```

## Parameters 

`streamRef`  

A valid stream.

## Discussion

Invalidates the stream, like CFRunLoopSourceInvalidate() does for a CFRunLoopSourceRef. It will be unscheduled from any runloops or dispatch queues upon which it had been scheduled.

FSEventStreamInvalidate() can only be called on the stream after you have called FSEventStreamScheduleWithRunLoop() or FSEventStreamSetDispatchQueue().

