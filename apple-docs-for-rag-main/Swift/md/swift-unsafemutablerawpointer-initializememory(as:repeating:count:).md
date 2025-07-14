

- Swift
- UnsafeMutableRawPointer
-  initializeMemory(as:repeating:count:) 

Instance Method

# initializeMemory(as:repeating:count:)

Initializes the memory referenced by this pointer with the given value, binds the memory to the value’s type, and returns a typed pointer to the initialized memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
func initializeMemory(
    as type: T.Type,
    repeating repeatedValue: T,
    count: Int
) -> UnsafeMutablePointer
```

## Parameters 

`type`  

The type to bind this memory to.

`repeatedValue`  

The instance to copy into memory.

`count`  

The number of copies of `value` to copy into memory. `count` must not be negative.

## Return Value

A typed pointer to the memory referenced by this raw pointer.

## Discussion

The memory referenced by this pointer must be uninitialized or initialized to a trivial type, and must be properly aligned for accessing `T`.

The following example allocates enough raw memory to hold four instances of `Int8`, and then uses the `initializeMemory(as:repeating:count:)` method to initialize the allocated memory.

```
let count = 4
let bytesPointer = UnsafeMutableRawPointer.allocate(
        byteCount: count * MemoryLayout.stride,
        alignment: MemoryLayout.alignment)
let int8Pointer = bytesPointer.initializeMemory(
        as: Int8.self, repeating: 0, count: count)

// After using 'int8Pointer':
int8Pointer.deallocate()
```

After calling this method on a raw pointer `p`, the region starting at `self` and continuing up to `p + count * MemoryLayout.stride` is bound to type `T` and initialized. If `T` is a nontrivial type, you must eventually deinitialize or move from the values in this region to avoid leaks.

