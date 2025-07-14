

- Swift
- UnsafeMutableRawBufferPointer
-  init(\_:) 

Initializer

# init(\_:)

Creates a raw buffer over the contiguous bytes in the given typed buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ buffer: UnsafeMutableBufferPointer) where T : ~Copyable
```

## Parameters 

`buffer`  

The typed buffer to convert to a raw buffer. The buffer’s type `T` must be a trivial type.

