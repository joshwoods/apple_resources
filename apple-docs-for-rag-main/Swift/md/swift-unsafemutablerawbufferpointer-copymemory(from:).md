

- Swift
- UnsafeMutableRawBufferPointer
-  copyMemory(from:) 

Instance Method

# copyMemory(from:)

Copies the bytes from the given buffer to this buffer’s memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func copyMemory(from source: UnsafeRawBufferPointer)
```

## Parameters 

`source`  

A buffer of raw bytes. `source.count` must be less than or equal to this buffer’s `count`.

## Discussion

If the `source.count` bytes of memory referenced by this buffer are bound to a type `T`, then `T` must be a trivial type, the underlying pointer must be properly aligned for accessing `T`, and `source.count` must be a multiple of `MemoryLayout.stride`.

The memory referenced by `source` may overlap with the memory referenced by this buffer.

After calling `copyMemory(from:)`, the first `source.count` bytes of memory referenced by this buffer are initialized to raw bytes. If the memory is bound to type `T`, then it contains values of type `T`.

