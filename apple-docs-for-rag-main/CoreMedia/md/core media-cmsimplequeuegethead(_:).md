

- Core Media
-  CMSimpleQueueGetHead(\_:) 

Function

# CMSimpleQueueGetHead(\_:)

Returns the element at the head of the queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSimpleQueueGetHead(_ queue: CMSimpleQueue) -> UnsafeRawPointer?
```

## Parameters 

`queue`  

The queue from which to get the head element. Must not be `NULL`.

## Return Value

The head element. `NULL` if the queue was empty, or if there was some other error.

## Discussion

If the queue is empty, the function returns `NULL`.

## See Also

### Inspecting Queues

func CMSimpleQueueGetCapacity(CMSimpleQueue) -> Int32

Returns the number of elements that the queue can hold.

func CMSimpleQueueGetCount(CMSimpleQueue) -> Int32

Returns the number of elements currently in the queue.

