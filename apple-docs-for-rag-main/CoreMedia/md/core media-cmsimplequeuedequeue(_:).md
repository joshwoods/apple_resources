

- Core Media
-  CMSimpleQueueDequeue(\_:) 

Function

# CMSimpleQueueDequeue(\_:)

Dequeues an element from the queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSimpleQueueDequeue(_ queue: CMSimpleQueue) -> UnsafeRawPointer?
```

## Parameters 

`queue`  

The queue from which to dequeue an element. Must not be `NULL`.

## Return Value

The dequeued element. `NULL` if the queue was empty, or if there was some other error.

## See Also

### Managing Queues

func CMSimpleQueueEnqueue(CMSimpleQueue, element: UnsafeRawPointer) -> OSStatus

Enqueues an element in the queue.

func CMSimpleQueueReset(CMSimpleQueue) -> OSStatus

Resets the queue.

