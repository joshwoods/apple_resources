

- Swift
- UnsafeRawBufferPointer
-  init(start:count:) 

Initializer

# init(start:count:)

Creates a buffer over the specified number of contiguous bytes starting at the given pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    start: UnsafeRawPointer?,
    count: Int
)
```

## Parameters 

`start`  

The address of the memory that starts the buffer. If `starts` is `nil`, `count` must be zero. However, `count` may be zero even for a non-`nil` `start`.

`count`  

The number of bytes to include in the buffer. `count` must not be negative.

