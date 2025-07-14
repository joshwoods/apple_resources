

- Core Media
-  CMSimpleQueueGetCapacity(\_:) 

Function

# CMSimpleQueueGetCapacity(\_:)

Returns the number of elements that the queue can hold.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSimpleQueueGetCapacity(_ queue: CMSimpleQueue) -> Int32
```

## Parameters 

`queue`  

The queue the function is interrogating. Must not be `NULL`.

## Return Value

The number of elements that the queue can hold. Returns `0` if there is an error.

## See Also

### Inspecting Queues

func CMSimpleQueueGetHead(CMSimpleQueue) -> UnsafeRawPointer?

Returns the element at the head of the queue.

func CMSimpleQueueGetCount(CMSimpleQueue) -> Int32

Returns the number of elements currently in the queue.

