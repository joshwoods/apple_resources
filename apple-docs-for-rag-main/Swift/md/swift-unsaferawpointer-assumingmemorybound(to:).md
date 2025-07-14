

- Swift
- UnsafeRawPointer
-  assumingMemoryBound(to:) 

Instance Method

# assumingMemoryBound(to:)

Returns a typed pointer to the memory referenced by this pointer, assuming that the memory is already bound to the specified type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func assumingMemoryBound(to: T.Type) -> UnsafePointer where T : ~Copyable
```

## Parameters 

`to`  

The type `T` that the memory has already been bound to.

## Return Value

A typed pointer to the same memory as this raw pointer.

## Discussion

Use this method when you have a raw pointer to memory that has *already* been bound to the specified type. The memory starting at this pointer must be bound to the type `T`. Accessing memory through the returned pointer is undefined if the memory has not been bound to `T`. To bind memory to `T`, use `bindMemory(to:capacity:)` instead of this method.

