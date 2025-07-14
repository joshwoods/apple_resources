

- Core Media
-  CMBufferQueueIsAtEndOfData(\_:) 

Function

# CMBufferQueueIsAtEndOfData(\_:)

Returns a Boolean value that indicates whether a buffer queue has its end-of-data marker set, and is now empty.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueIsAtEndOfData(_ queue: CMBufferQueue) -> Bool
```

## Parameters 

`queue`  

The `CMBufferQueue` being interrogated.

## Return Value

A Boolean indicating whether the `CMBufferQueue` has been marked with EndOfData, and is now empty.If queue is `NULL`, true is returned (a NULL queue is considered to be empty, and permanently at EndOfData).

## See Also

### Inspecting a Queue

func CMBufferQueueIsEmpty(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue is empty.

func CMBufferQueueGetBufferCount(CMBufferQueue) -> CMItemCount

Gets the number of buffers in the queue.

func CMBufferQueueGetTotalSize(CMBufferQueue) -> Int

Gets the total size of all sample buffers of a buffer queue.

func CMBufferQueueGetHead(CMBufferQueue) -> CMBuffer?

Retrieves the next buffer from a queue, but doesn’t remove it.

Deprecated

func CMBufferQueueContainsEndOfData(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue has its end-of-data marker set.

