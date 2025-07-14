

- Core Media
-  CMSimpleQueueReset(\_:) 

Function

# CMSimpleQueueReset(\_:)

Resets the queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSimpleQueueReset(_ queue: CMSimpleQueue) -> OSStatus
```

## Parameters 

`queue`  

The queue to reset. Must not be `NULL`.

## Return Value

Returns `noErr` if the call succeeds.

## Discussion

This function resets the queue to an empty state. `CMSimpleQueueReset` isn’t synchronized in any way, so the client must hold off the reader thread and writer thread during this operation.

## See Also

### Managing Queues

func CMSimpleQueueEnqueue(CMSimpleQueue, element: UnsafeRawPointer) -> OSStatus

Enqueues an element in the queue.

func CMSimpleQueueDequeue(CMSimpleQueue) -> UnsafeRawPointer?

Dequeues an element from the queue.

