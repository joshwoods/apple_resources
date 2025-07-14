

- Core Media
-  CMBufferQueueDequeueIfDataReady(\_:) 

Function

# CMBufferQueueDequeueIfDataReady(\_:)

Dequeues a buffer from a queue, if it’s ready.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueDequeueIfDataReady(_ queue: CMBufferQueue) -> CMBuffer?
```

## Parameters 

`queue`  

The `CMBufferQueue` from which to dequeue a buffer (if the buffer is ready).

## Return Value

The dequeued buffer. Will be `NULL` if the queue is empty, or if the buffer to be dequeued is not yet ready.

## Discussion

The buffer is released by the queue, but it is also retained for the client. Buffer ownership is thereby transferred from queue to client. The client need not retain the buffer, but is responsible to release it when done with it.

## See Also

### Managing a Queue

func CMBufferQueueEnqueue(CMBufferQueue, buffer: CMBuffer) -> OSStatus

Enqueues a buffer onto a queue.

func CMBufferQueueCallForEachBuffer(CMBufferQueue, callback: (CMBuffer, UnsafeMutableRawPointer?) -> OSStatus, refcon: UnsafeMutableRawPointer?) -> OSStatus

Calls a function for every buffer in a queue.

func CMBufferQueueDequeue(CMBufferQueue) -> CMBuffer?

Dequeues a buffer from a queue.

func CMBufferQueueMarkEndOfData(CMBufferQueue) -> OSStatus

Sets a marker to indicate this queue doesn’t allow enqueuing new buffers.

func CMBufferQueueReset(CMBufferQueue) -> OSStatus

Resets a buffer queue, which allows it to enqueue new buffers.

func CMBufferQueueResetWithCallback(CMBufferQueue, callback: (CMBuffer, UnsafeMutableRawPointer?) -> Void, refcon: UnsafeMutableRawPointer?) -> OSStatus

A callback that invokes a function for every buffer in a queue and then resets the queue.

func CMBufferQueueRemoveTrigger(CMBufferQueue, triggerToken: CMBufferQueueTriggerToken) -> OSStatus

Removes a previously installed trigger from a buffer queue.

