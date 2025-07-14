

- Core Media
-  CMSimpleQueueGetCount(\_:) 

Function

# CMSimpleQueueGetCount(\_:)

Returns the number of elements currently in the queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSimpleQueueGetCount(_ queue: CMSimpleQueue) -> Int32
```

## Parameters 

`queue`  

The queue the function is interrogating. Must not be `NULL`.

## Return Value

The number of elements currently in the queue. Returns `0` if there is an error.

## See Also

### Inspecting Queues

func CMSimpleQueueGetHead(CMSimpleQueue) -> UnsafeRawPointer?

Returns the element at the head of the queue.

func CMSimpleQueueGetCapacity(CMSimpleQueue) -> Int32

Returns the number of elements that the queue can hold.

