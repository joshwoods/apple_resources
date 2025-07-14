

- IOKit
- IOKit Functions
-  IOCFUnserialize(\_:\_:\_:\_:) 

Function

# IOCFUnserialize(\_:\_:\_:\_:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 13.0+macOS 10.0+visionOS 2.4+

``` source
func IOCFUnserialize(
    _ buffer: UnsafePointer!,
    _ allocator: CFAllocator!,
    _ options: CFOptionFlags,
    _ errorString: UnsafeMutablePointer?>!
) -> CFTypeRef!
```

