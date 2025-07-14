

- Swift
- UnsafeMutablePointer
-  moveInitialize(from:count:) 

Instance Method

# moveInitialize(from:count:)

Moves instances from initialized source memory into the uninitialized memory referenced by this pointer, leaving the source memory uninitialized and the memory referenced by this pointer initialized.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func moveInitialize(
    from source: UnsafeMutablePointer,
    count: Int
)
```

## Parameters 

`source`  

A pointer to the values to copy. The memory region `source..

`count`  

The number of instances to move from `source` to this pointer’s memory. `count` must not be negative.

## Discussion

The region of memory starting at this pointer and covering `count` instances of the pointer’s `Pointee` type must be uninitialized or `Pointee` must be a trivial type. After calling `moveInitialize(from:count:)`, the region is initialized and the memory region `source..

