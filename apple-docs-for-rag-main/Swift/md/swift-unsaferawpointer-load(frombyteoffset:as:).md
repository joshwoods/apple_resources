

- Swift
- UnsafeRawPointer
-  load(fromByteOffset:as:) 

Instance Method

# load(fromByteOffset:as:)

Returns a new instance of the given type, constructed from the raw memory at the specified offset.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func load(
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

A new instance of type `T`, read from the raw bytes at `offset`. The returned instance is memory-managed and unassociated with the value in the memory referenced by this pointer.

## Discussion

The memory at this pointer plus `offset` must be properly aligned for accessing `T` and initialized to `T` or another type that is layout compatible with `T`.

