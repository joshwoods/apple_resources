

- Swift
- UnsafeMutablePointer
-  update(from:count:) 

Instance Method

# update(from:count:)

Update this pointer’s initialized memory with the specified number of instances, copied from the given pointer’s memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func update(
    from source: UnsafePointer,
    count: Int
)
```

## Parameters 

`source`  

A pointer to at least `count` initialized instances of type `Pointee`. The memory regions referenced by `source` and this pointer may overlap.

`count`  

The number of instances to copy from the memory referenced by `source` to this pointer’s memory. `count` must not be negative.

## Discussion

The region of memory starting at this pointer and covering `count` instances of the pointer’s `Pointee` type must be initialized or `Pointee` must be a trivial type. After calling `update(from:count:)`, the region is initialized.

Note

Returns without performing work if `self` and `source` are equal.

