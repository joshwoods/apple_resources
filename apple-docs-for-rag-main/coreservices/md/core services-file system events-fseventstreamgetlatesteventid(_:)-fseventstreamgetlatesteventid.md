

- Core Services
- File System Events
-  FSEventStreamGetLatestEventId(\_:) 

Function

# FSEventStreamGetLatestEventId(\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func FSEventStreamGetLatestEventId(_ streamRef: ConstFSEventStreamRef) -> FSEventStreamEventId
```

## Parameters 

`streamRef`  

A valid stream.

## Return Value

The sinceWhen attribute of the stream.

## Discussion

Fetches the sinceWhen property of the stream. Upon receiving an event (and just before invoking the client's callback) this attribute is updated to the highest-numbered event ID mentioned in the event.

