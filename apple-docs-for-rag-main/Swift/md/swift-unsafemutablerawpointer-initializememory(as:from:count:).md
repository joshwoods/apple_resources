

- Swift
- UnsafeMutableRawPointer
-  initializeMemory(as:from:count:) 

Instance Method

# initializeMemory(as:from:count:)

Initializes the memory referenced by this pointer with the values starting at the given pointer, binds the memory to the values’ type, and returns a typed pointer to the initialized memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
func initializeMemory(
    as type: T.Type,
    from source: UnsafePointer,
    count: Int
) -> UnsafeMutablePointer
```

## Parameters 

`type`  

The type to bind this memory to.

`source`  

A pointer to the values to copy. The memory in the region `source..

`count`  

The number of copies of `value` to copy into memory. `count` must not be negative.

## Return Value

A typed pointer to the memory referenced by this raw pointer.

## Discussion

The memory referenced by this pointer must be uninitialized or initialized to a trivial type, and must be properly aligned for accessing `T`.

The following example allocates enough raw memory to hold four instances of `Int8`, and then uses the `initializeMemory(as:from:count:)` method to initialize the allocated memory.

```
let count = 4
let bytesPointer = UnsafeMutableRawPointer.allocate(
        byteCount: count * MemoryLayout.stride,
        alignment: MemoryLayout.alignment)
let values: [Int8] = [1, 2, 3, 4]
let int8Pointer = values.withUnsafeBufferPointer { buffer in
    return bytesPointer.initializeMemory(as: Int8.self,
              from: buffer.baseAddress!,
              count: buffer.count)
}
// int8Pointer.pointee == 1
// (int8Pointer + 3).pointee == 4

// After using 'int8Pointer':
int8Pointer.deallocate()
```

After calling this method on a raw pointer `p`, the region starting at `p` and continuing up to `p + count * MemoryLayout.stride` is bound to type `T` and initialized. If `T` is a nontrivial type, you must eventually deinitialize or move from the values in this region to avoid leaks. The instances in the region `source..

