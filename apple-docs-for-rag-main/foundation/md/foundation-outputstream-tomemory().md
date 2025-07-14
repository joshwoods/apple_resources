

- Foundation
- OutputStream
-  toMemory() 

Type Method

# toMemory()

Creates and returns an initialized output stream that will write stream data to memory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func toMemory() -> Self
```

## Return Value

An initialized output stream that will write stream data to memory.

## Discussion

The stream must be opened before it can be used.

You retrieve the contents of the memory stream by sending the message property(forKey:) to the receiver with an argument of `NSStreamDataWrittenToMemoryStreamKey`.

## See Also

### Related Documentation

Stream Programming Guide

### Creating Streams

convenience init?(URL: URL, append: Bool)

Creates and returns an initialized output stream for writing to a specified URL.

init(toMemory: ())

Returns an initialized output stream that will write to memory.

init(toBuffer: UnsafeMutablePointer&lt;UInt8>, capacity: Int)

Returns an initialized output stream that can write to a provided buffer.

convenience init?(toFileAtPath: String, append: Bool)

Returns an initialized output stream for writing to a specified file.

init?(url: URL, append: Bool)

Returns an initialized output stream for writing to a specified URL.

