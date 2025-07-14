

- Swift
- StringProtocol
-  init(cString:) 

Initializer

# init(cString:)

Creates a string from the null-terminated, UTF-8 encoded sequence of bytes at the given pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(cString nullTerminatedUTF8: UnsafePointer)
```

**Required**

## Parameters 

`nullTerminatedUTF8`  

A pointer to a sequence of contiguous, UTF-8 encoded bytes ending just before the first zero byte.

