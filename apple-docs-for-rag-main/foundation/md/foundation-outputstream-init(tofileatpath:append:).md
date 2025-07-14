

- Foundation
- OutputStream
-  init(toFileAtPath:append:) 

Initializer

# init(toFileAtPath:append:)

Returns an initialized output stream for writing to a specified file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(
    toFileAtPath path: String,
    append shouldAppend: Bool
)
```

## Parameters 

`path`  

The path to the file the output stream will write to.

`shouldAppend`  

true if newly written data should be appended to any existing file contents, otherwise false.

## Return Value

An initialized output stream that can write to `path`.

## Discussion

The stream must be opened before it can be used.

## See Also

### Related Documentation

convenience init?(URL: URL, append: Bool)

Creates and returns an initialized output stream for writing to a specified URL.

### Creating Streams

class func toMemory() -> Self

Creates and returns an initialized output stream that will write stream data to memory.

convenience init?(URL: URL, append: Bool)

Creates and returns an initialized output stream for writing to a specified URL.

init(toMemory: ())

Returns an initialized output stream that will write to memory.

init(toBuffer: UnsafeMutablePointer&lt;UInt8>, capacity: Int)

Returns an initialized output stream that can write to a provided buffer.

init?(url: URL, append: Bool)

Returns an initialized output stream for writing to a specified URL.

