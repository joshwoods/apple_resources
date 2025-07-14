

- Core Services
- File System Events
-  FSEventStreamFlushSync(\_:) 

Function

# FSEventStreamFlushSync(\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func FSEventStreamFlushSync(_ streamRef: FSEventStreamRef)
```

## Parameters 

`streamRef`  

A valid stream.

## Discussion

Asks the FS Events service to flush out any events that have occurred but have not yet been delivered, due to the latency parameter that was supplied when the stream was created. This flushing occurs synchronously -- by the time this call returns, your callback will have been invoked for every event that had already occurred at the time you made this call.

FSEventStreamFlushSync() can only be called after the stream has been started, via FSEventStreamStart().

