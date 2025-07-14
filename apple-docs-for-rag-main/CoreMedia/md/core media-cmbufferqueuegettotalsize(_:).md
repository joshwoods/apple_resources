

- Core Media
-  CMBufferQueueGetTotalSize(\_:) 

Function

# CMBufferQueueGetTotalSize(\_:)

Gets the total size of all sample buffers of a buffer queue.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueGetTotalSize(_ queue: CMBufferQueue) -> Int
```

## Discussion

The total size of the `CMBufferQueue` is the sum of all the individual buffer sizes, as reported by the `getTotalSize` callback (provided to CMBufferQueueCreate(allocator:capacity:callbacks:queueOut:)).

This function returns 0 if there are no buffers in the queue.

## See Also

### Inspecting a Queue

func CMBufferQueueIsEmpty(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue is empty.

func CMBufferQueueGetBufferCount(CMBufferQueue) -> CMItemCount

Gets the number of buffers in the queue.

func CMBufferQueueGetHead(CMBufferQueue) -> CMBuffer?

Retrieves the next buffer from a queue, but doesn’t remove it.

Deprecated

func CMBufferQueueContainsEndOfData(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue has its end-of-data marker set.

func CMBufferQueueIsAtEndOfData(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue has its end-of-data marker set, and is now empty.

