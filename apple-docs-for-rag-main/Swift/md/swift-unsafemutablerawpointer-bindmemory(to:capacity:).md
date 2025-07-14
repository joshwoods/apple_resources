

- Swift
- UnsafeMutableRawPointer
-  bindMemory(to:capacity:) 

Instance Method

# bindMemory(to:capacity:)

Binds the memory to the specified type and returns a typed pointer to the bound memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
func bindMemory(
    to type: T.Type,
    capacity count: Int
) -> UnsafeMutablePointer where T : ~Copyable
```

## Parameters 

`type`  

The type `T` to bind the memory to.

`count`  

The amount of memory to bind to type `T`, counted as instances of `T`.

## Return Value

A typed pointer to the newly bound memory. The memory in this region is bound to `T`, but has not been modified in any other way. The number of bytes in this region is `count * MemoryLayout.stride`.

## Discussion

Use the `bindMemory(to:capacity:)` method to bind the memory referenced by this pointer to the type `T`. The memory must be uninitialized or initialized to a type that is layout compatible with `T`. If the memory is uninitialized, it is still uninitialized after being bound to `T`.

In this example, 100 bytes of raw memory are allocated for the pointer `bytesPointer`, and then the first four bytes are bound to the `Int8` type.

```
let count = 4
let bytesPointer = UnsafeMutableRawPointer.allocate(
        byteCount: 100,
        alignment: MemoryLayout.alignment)
let int8Pointer = bytesPointer.bindMemory(to: Int8.self, capacity: count)
```

After calling `bindMemory(to:capacity:)`, the first four bytes of the memory referenced by `bytesPointer` are bound to the `Int8` type, though they remain uninitialized. The remainder of the allocated region is unbound raw memory. All 100 bytes of memory must eventually be deallocated.

Warning

A memory location may only be bound to one type at a time. The behavior of accessing memory as a type unrelated to its bound type is undefined.

