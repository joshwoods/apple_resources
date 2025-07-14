

- Core Services
- File System Events
-  FSEventStreamStop(\_:) 

Function

# FSEventStreamStop(\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func FSEventStreamStop(_ streamRef: FSEventStreamRef)
```

## Parameters 

`streamRef`  

A valid stream.

## Discussion

Unregisters with the FS Events service. The client callback will not be called for this stream while it is stopped.

FSEventStreamStop() can only be called if the stream has been started, via FSEventStreamStart().

Once stopped, the stream can be restarted via FSEventStreamStart(), at which point it will resume receiving events from where it left off ("sinceWhen").

