

- Foundation
- OutputStream
-  init(toBuffer:capacity:) 

Initializer

# init(toBuffer:capacity:)

Returns an initialized output stream that can write to a provided buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    toBuffer buffer: UnsafeMutablePointer,
    capacity: Int
)
```

## Parameters 

`buffer`  

The buffer the output stream will write to.

`capacity`  

The size of the buffer in bytes.

## Return Value

An initialized output stream that can write to `buffer`.

## Discussion

The stream must be opened before it can be used.

When the number of bytes written to `buffer` has reached `capacity`, the stream’s streamStatus will return `NSStreamStatusAtEnd`.

## See Also

### Creating Streams

class func toMemory() -> Self

Creates and returns an initialized output stream that will write stream data to memory.

convenience init?(URL: URL, append: Bool)

Creates and returns an initialized output stream for writing to a specified URL.

init(toMemory: ())

Returns an initialized output stream that will write to memory.

convenience init?(toFileAtPath: String, append: Bool)

Returns an initialized output stream for writing to a specified file.

init?(url: URL, append: Bool)

Returns an initialized output stream for writing to a specified URL.

