

- Core Media
-  CMBufferQueueGetBufferCount(\_:) 

Function

# CMBufferQueueGetBufferCount(\_:)

Gets the number of buffers in the queue.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueGetBufferCount(_ queue: CMBufferQueue) -> CMItemCount
```

## Parameters 

`queue`  

`CMBufferQueue` being interrogated.

## Return Value

Returns the number of buffers in the `CMBufferQueue`.

## See Also

### Inspecting a Queue

func CMBufferQueueIsEmpty(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue is empty.

func CMBufferQueueGetTotalSize(CMBufferQueue) -> Int

Gets the total size of all sample buffers of a buffer queue.

func CMBufferQueueGetHead(CMBufferQueue) -> CMBuffer?

Retrieves the next buffer from a queue, but doesn’t remove it.

Deprecated

func CMBufferQueueContainsEndOfData(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue has its end-of-data marker set.

func CMBufferQueueIsAtEndOfData(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue has its end-of-data marker set, and is now empty.

