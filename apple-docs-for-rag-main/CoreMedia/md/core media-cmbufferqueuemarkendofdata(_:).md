

- Core Media
-  CMBufferQueueMarkEndOfData(\_:) 

Function

# CMBufferQueueMarkEndOfData(\_:)

Sets a marker to indicate this queue doesn’t allow enqueuing new buffers.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueMarkEndOfData(_ queue: CMBufferQueue) -> OSStatus
```

## Parameters 

`queue`  

The `CMBufferQueue` being marked.

## Return Value

A result code. See `Result Codes`

## Discussion

All subsequent Enqueues will be rejected until CMBufferQueueReset(_:) is called. Subsequent Dequeues will succeed as long as the queue is not empty.

## See Also

### Managing a Queue

func CMBufferQueueEnqueue(CMBufferQueue, buffer: CMBuffer) -> OSStatus

Enqueues a buffer onto a queue.

func CMBufferQueueCallForEachBuffer(CMBufferQueue, callback: (CMBuffer, UnsafeMutableRawPointer?) -> OSStatus, refcon: UnsafeMutableRawPointer?) -> OSStatus

Calls a function for every buffer in a queue.

func CMBufferQueueDequeue(CMBufferQueue) -> CMBuffer?

Dequeues a buffer from a queue.

func CMBufferQueueDequeueIfDataReady(CMBufferQueue) -> CMBuffer?

Dequeues a buffer from a queue, if it’s ready.

func CMBufferQueueReset(CMBufferQueue) -> OSStatus

Resets a buffer queue, which allows it to enqueue new buffers.

func CMBufferQueueResetWithCallback(CMBufferQueue, callback: (CMBuffer, UnsafeMutableRawPointer?) -> Void, refcon: UnsafeMutableRawPointer?) -> OSStatus

A callback that invokes a function for every buffer in a queue and then resets the queue.

func CMBufferQueueRemoveTrigger(CMBufferQueue, triggerToken: CMBufferQueueTriggerToken) -> OSStatus

Removes a previously installed trigger from a buffer queue.

