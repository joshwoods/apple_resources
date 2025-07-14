

- IOKit
- IOKit Functions
-  IOCFUnserializeBinary(\_:\_:\_:\_:\_:) 

Function

# IOCFUnserializeBinary(\_:\_:\_:\_:\_:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 13.0+macOS 10.10+visionOS 2.4+

``` source
func IOCFUnserializeBinary(
    _ buffer: UnsafePointer!,
    _ bufferSize: Int,
    _ allocator: CFAllocator!,
    _ options: CFOptionFlags,
    _ errorString: UnsafeMutablePointer?>!
) -> CFTypeRef!
```

