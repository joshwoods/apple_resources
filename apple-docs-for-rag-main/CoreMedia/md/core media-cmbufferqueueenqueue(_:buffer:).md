

- Core Media
-  CMBufferQueueEnqueue(\_:buffer:) 

Function

# CMBufferQueueEnqueue(\_:buffer:)

Enqueues a buffer onto a queue.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueEnqueue(
    _ queue: CMBufferQueue,
    buffer buf: CMBuffer
) -> OSStatus
```

## Parameters 

`queue`  

The `CMBufferQueue` on which to enqueue the buffer.

`buf`  

The buffer to enqueue.

## Return Value

A result code. See `Result Codes`.

## Discussion

The buffer is retained by the queue, so the client can safely release the buffer if it has no further use for it. If the compare callback is non-`NULL`, this API performs an insertion sort using that compare operation. If the validation callback is non-`NULL`, this API calls it; if it returns a nonzero `OSStatus`, the buffer will not be enqueued and this API will return the same error `OSStatus`.

## See Also

### Managing a Queue

func CMBufferQueueCallForEachBuffer(CMBufferQueue, callback: (CMBuffer, UnsafeMutableRawPointer?) -> OSStatus, refcon: UnsafeMutableRawPointer?) -> OSStatus

Calls a function for every buffer in a queue.

func CMBufferQueueDequeue(CMBufferQueue) -> CMBuffer?

Dequeues a buffer from a queue.

func CMBufferQueueDequeueIfDataReady(CMBufferQueue) -> CMBuffer?

Dequeues a buffer from a queue, if it’s ready.

func CMBufferQueueMarkEndOfData(CMBufferQueue) -> OSStatus

Sets a marker to indicate this queue doesn’t allow enqueuing new buffers.

func CMBufferQueueReset(CMBufferQueue) -> OSStatus

Resets a buffer queue, which allows it to enqueue new buffers.

func CMBufferQueueResetWithCallback(CMBufferQueue, callback: (CMBuffer, UnsafeMutableRawPointer?) -> Void, refcon: UnsafeMutableRawPointer?) -> OSStatus

A callback that invokes a function for every buffer in a queue and then resets the queue.

func CMBufferQueueRemoveTrigger(CMBufferQueue, triggerToken: CMBufferQueueTriggerToken) -> OSStatus

Removes a previously installed trigger from a buffer queue.

