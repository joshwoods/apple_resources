

- Core Media
- CMBlockBufferCustomBlockSource
-  version 

Instance Property

# version

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
var version: UInt32
```

## See Also

### Properties

var AllocateBlock: ((UnsafeMutableRawPointer?, Int) -> UnsafeMutableRawPointer?)?

The function to allocate memory.

var FreeBlock: ((UnsafeMutableRawPointer?, UnsafeMutableRawPointer, Int) -> Void)?

A function to call once when the `CMBlockBuffer` is disposed.

var refCon: UnsafeMutableRawPointer?

Contextual information passed to both the allocate and free function calls.

