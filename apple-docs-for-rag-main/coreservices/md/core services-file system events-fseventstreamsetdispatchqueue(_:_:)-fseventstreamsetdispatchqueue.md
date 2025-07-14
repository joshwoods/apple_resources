

- Core Services
- File System Events
-  FSEventStreamSetDispatchQueue(\_:\_:) 

Function

# FSEventStreamSetDispatchQueue(\_:\_:)

Schedules the stream on the specified dispatch queue.

Mac Catalyst 13.1+macOS 10.6+

``` source
func FSEventStreamSetDispatchQueue(
    _ streamRef: FSEventStreamRef,
    _ q: dispatch_queue_t?
)
```

## Parameters 

`streamRef`  

A valid stream.

`q`  

The dispatch queue to use to receive events (or `NULL` to stop receiving events from the stream).

## Discussion

The caller is responsible for ensuring that the stream is scheduled on a dispatch queue and that the queue is started.

If there’s a problem scheduling the stream on the queue, an error will be returned when you try to start the stream.

To start receiving events on the stream, call FSEventStreamStart(_:).

To remove the stream from the queue on which it was scheduled, call FSEventStreamSetDispatchQueue(_:_:) with a `NULL` queue parameter or call FSEventStreamInvalidate(_:) which does the same thing. You must eventually call `FSEventStreamInvalidate(_:)` and it’s an error to call `FSEventStreamInvalidate(_:)` without having the stream either scheduled on a runloop or a dispatch queue, so don’t set the dispatch queue to `NULL` before calling `FSEventStreamInvalidate(_:)`.

