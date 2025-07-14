

- Core Media
-  CMBufferQueueGetHead(\_:) Deprecated

Function

# CMBufferQueueGetHead(\_:)

Retrieves the next buffer from a queue, but doesn’t remove it.

iOS 4.0–18.0DeprecatediPadOS 4.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.0–11.0Deprecated

``` source
func CMBufferQueueGetHead(_ queue: CMBufferQueue) -> CMBuffer?
```

## Parameters 

`queue`  

The CMBufferQueue from which to retrieve a buffer.

## Return Value

The buffer. Will be `NULL` if the queue is empty.

## Discussion

This follows Core Foundation “Get” semantics – it does not retain the returned buffer. Note that with non-FIFO queues it’s not guaranteed that the next dequeue will return this particular buffer (if an intervening Enqueue adds a buffer that will dequeue next).

## See Also

### Inspecting a Queue

func CMBufferQueueIsEmpty(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue is empty.

func CMBufferQueueGetBufferCount(CMBufferQueue) -> CMItemCount

Gets the number of buffers in the queue.

func CMBufferQueueGetTotalSize(CMBufferQueue) -> Int

Gets the total size of all sample buffers of a buffer queue.

func CMBufferQueueContainsEndOfData(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue has its end-of-data marker set.

func CMBufferQueueIsAtEndOfData(CMBufferQueue) -> Bool

Returns a Boolean value that indicates whether a buffer queue has its end-of-data marker set, and is now empty.

