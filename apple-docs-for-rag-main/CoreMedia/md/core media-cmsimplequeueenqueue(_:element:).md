

- Core Media
-  CMSimpleQueueEnqueue(\_:element:) 

Function

# CMSimpleQueueEnqueue(\_:element:)

Enqueues an element in the queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSimpleQueueEnqueue(
    _ queue: CMSimpleQueue,
    element: UnsafeRawPointer
) -> OSStatus
```

## Parameters 

`queue`  

The queue on which to enqueue the element. Must not be `NULL`.

`element`  

Element to enqueue. Must not be `NULL` (`CMSimpleQueueDequeue` returns `NULL` to indicate an empty queue).

## Return Value

Returns `noErr` if the call succeeds or `kCMSimpleQueueError_QueueIsFull` if the queue is full.

## Discussion

If the queue is full, this operation fails.

## See Also

### Managing Queues

func CMSimpleQueueDequeue(CMSimpleQueue) -> UnsafeRawPointer?

Dequeues an element from the queue.

func CMSimpleQueueReset(CMSimpleQueue) -> OSStatus

Resets the queue.

