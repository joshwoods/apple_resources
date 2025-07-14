

- Swift
- UnsafeMutableRawPointer
-  copyMemory(from:byteCount:) 

Instance Method

# copyMemory(from:byteCount:)

Copies the specified number of bytes from the given raw pointer’s memory into this pointer’s memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func copyMemory(
    from source: UnsafeRawPointer,
    byteCount: Int
)
```

## Parameters 

`source`  

A pointer to the memory to copy bytes from. The memory in the region `source..

`byteCount`  

The number of bytes to copy. `byteCount` must not be negative.

## Discussion

If the `byteCount` bytes of memory referenced by this pointer are bound to a type `T`, then `T` must be a trivial type, this pointer and `source` must be properly aligned for accessing `T`, and `byteCount` must be a multiple of `MemoryLayout.stride`.

The memory in the region `source..

