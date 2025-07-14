

- Swift
- UnsafeBufferPointer
-  init(start:count:) 

Initializer

# init(start:count:)

Creates a new buffer pointer over the specified number of contiguous instances beginning at the given pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    start: UnsafePointer?,
    count: Int
)
```

## Parameters 

`start`  

A pointer to the start of the buffer, or `nil`. If `start` is `nil`, `count` must be zero. However, `count` may be zero even for a non-`nil` `start`. The pointer passed as `start` must be aligned to `MemoryLayout.alignment`.

`count`  

The number of instances in the buffer. `count` must not be negative.

