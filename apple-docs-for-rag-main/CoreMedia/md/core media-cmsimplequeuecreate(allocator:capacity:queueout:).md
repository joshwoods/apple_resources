

- Core Media
-  CMSimpleQueueCreate(allocator:capacity:queueOut:) 

Function

# CMSimpleQueueCreate(allocator:capacity:queueOut:)

Creates a queue that has the specified capacity.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSimpleQueueCreate(
    allocator: CFAllocator?,
    capacity: Int32,
    queueOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator used to allocate storage for the queue.

`capacity`  

Capacity of the queue (maximum number of elements holdable at any given time). Required (must not be `0`). Must be a positive value.

`queueOut`  

On output, a reference to the newly created queue. Must not be `NULL`.

## Return Value

A result code. See Simple Queue Error Codes.

## Discussion

On return, the caller owns the returned `CMSimpleQueue`, and must release it when done with it.

