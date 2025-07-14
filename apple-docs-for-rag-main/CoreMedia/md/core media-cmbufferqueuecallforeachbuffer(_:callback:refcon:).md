

- Core Media
-  CMBufferQueueCallForEachBuffer(\_:callback:refcon:) 

Function

# CMBufferQueueCallForEachBuffer(\_:callback:refcon:)

Calls a function for every buffer in a queue.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueCallForEachBuffer(
    _ queue: CMBufferQueue,
    callback: (CMBuffer, UnsafeMutableRawPointer?) -> OSStatus,
    refcon: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`queue`  

`CMBufferQueue` that may contain multiple buffers.

`callback`  

Function to be called for each buffer. The callback may modify buffer attachments but should not modify sort-affecting properties (eg, timestamps). The callback should not make other calls to the buffer queue.

`refcon`  

Reference constant supplied to the callback function.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

If the callback function returns an error, iteration will stop immediately and the error will be returned.

## See Also

### Managing a Queue

func CMBufferQueueEnqueue(CMBufferQueue, buffer: CMBuffer) -> OSStatus

Enqueues a buffer onto a queue.

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

