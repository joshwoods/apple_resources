

- Swift
- UnsafeMutablePointer
-  moveUpdate(from:count:) 

Instance Method

# moveUpdate(from:count:)

Update this pointer’s initialized memory by moving the specified number of instances the source pointer’s memory, leaving the source memory uninitialized.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func moveUpdate(
    from source: UnsafeMutablePointer,
    count: Int
)
```

## Parameters 

`source`  

A pointer to the values to be moved. The memory region `source..

`count`  

The number of instances to move from `source` to this pointer’s memory. `count` must not be negative.

## Discussion

The region of memory starting at this pointer and covering `count` instances of the pointer’s `Pointee` type must be initialized or `Pointee` must be a trivial type. After calling `moveUpdate(from:count:)`, the region is initialized and the memory region `source..

