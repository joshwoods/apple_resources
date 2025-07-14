

- Foundation
- OutputStream
-  init(toMemory:) 

Initializer

# init(toMemory:)

Returns an initialized output stream that will write to memory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(toMemory: ())
```

## Return Value

An initialized output stream that will write stream data to memory.

## Discussion

The stream must be opened before it can be used.

The contents of the memory stream are retrieved by passing the constant `NSStreamDataWrittenToMemoryStreamKey` to property(forKey:).

## See Also

### Creating Streams

class func toMemory() -> Self

Creates and returns an initialized output stream that will write stream data to memory.

convenience init?(URL: URL, append: Bool)

Creates and returns an initialized output stream for writing to a specified URL.

init(toBuffer: UnsafeMutablePointer&lt;UInt8>, capacity: Int)

Returns an initialized output stream that can write to a provided buffer.

convenience init?(toFileAtPath: String, append: Bool)

Returns an initialized output stream for writing to a specified file.

init?(url: URL, append: Bool)

Returns an initialized output stream for writing to a specified URL.

