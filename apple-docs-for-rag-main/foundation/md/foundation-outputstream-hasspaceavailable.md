

- Foundation
- OutputStream
-  hasSpaceAvailable 

Instance Property

# hasSpaceAvailable

A boolean value that indicates whether the receiver can be written to.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hasSpaceAvailable: Bool { get }
```

## Discussion

true if the receiver can be written to or if a write must be attempted in order to determine if space is available, false otherwise.

## See Also

### Using Streams

func write(UnsafePointer&lt;UInt8>, maxLength: Int) -> Int

Writes the contents of a provided data buffer to the receiver.

