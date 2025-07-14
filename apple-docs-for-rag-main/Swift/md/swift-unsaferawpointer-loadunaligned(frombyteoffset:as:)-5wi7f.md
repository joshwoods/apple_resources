

- Swift
- UnsafeRawPointer
-  loadUnaligned(fromByteOffset:as:) 

Instance Method

# loadUnaligned(fromByteOffset:as:)

Returns a new instance of the given type, constructed from the raw memory at the specified offset.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func loadUnaligned(
    fromByteOffset offset: Int = 0,
    as type: T.Type
) -> T
```

## Parameters 

`offset`  

The offset from this pointer, in bytes. `offset` must be nonnegative. The default is zero.

`type`  

The type of the instance to create.

## Return Value

A new instance of type `T`, read from the raw bytes at `offset`. The returned instance isn’t associated with the value in the range of memory referenced by this pointer.

## Discussion

This function only supports loading trivial types, and will trap if this precondition is not met. A trivial type does not contain any reference-counted property within its in-memory representation. The memory at this pointer plus `offset` must be laid out identically to the in-memory representation of `T`.

Note

A trivial type can be copied with just a bit-for-bit copy without any indirection or reference-counting operations. Generally, native Swift types that do not contain strong or weak references or other forms of indirection are trivial, as are imported C structs and enums.

