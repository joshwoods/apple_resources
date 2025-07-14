

- Swift
- UnsafeMutableRawBufferPointer
-  initializeMemory(as:repeating:) 

Instance Method

# initializeMemory(as:repeating:)

Initializes the memory referenced by this buffer with the given value, binds the memory to the value’s type, and returns a typed buffer of the initialized memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
func initializeMemory(
    as type: T.Type,
    repeating repeatedValue: T
) -> UnsafeMutableBufferPointer
```

## Parameters 

`type`  

The type to bind this buffer’s memory to.

`repeatedValue`  

The instance to copy into memory.

## Return Value

A typed buffer of the memory referenced by this raw buffer. The typed buffer contains `self.count / MemoryLayout.stride` instances of `T`.

## Discussion

The memory referenced by this buffer must be uninitialized or initialized to a trivial type, and must be properly aligned for accessing `T`.

After calling this method on a raw buffer with non-nil `baseAddress` `b`, the region starting at `b` and continuing up to `b + self.count - self.count % MemoryLayout.stride` is bound to type `T` and is initialized. If `T` is a nontrivial type, you must eventually deinitialize or move the values in this region to avoid leaks. If `baseAddress` is `nil`, this function does nothing and returns an empty buffer pointer.

