

- Foundation
- OutputStream
-  init(URL:append:) 

Initializer

# init(URL:append:)

Creates and returns an initialized output stream for writing to a specified URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(
    URL url: URL,
    append shouldAppend: Bool
)
```

## Parameters 

`url`  

The URL to the file the output stream will write to.

`shouldAppend`  

true if newly written data should be appended to any existing file contents, otherwise false.

## Return Value

An initialized output stream that can write to `url`.

## Discussion

The stream must be opened before it can be used.

## See Also

### Creating Streams

class func toMemory() -> Self

Creates and returns an initialized output stream that will write stream data to memory.

init(toMemory: ())

Returns an initialized output stream that will write to memory.

init(toBuffer: UnsafeMutablePointer&lt;UInt8>, capacity: Int)

Returns an initialized output stream that can write to a provided buffer.

convenience init?(toFileAtPath: String, append: Bool)

Returns an initialized output stream for writing to a specified file.

init?(url: URL, append: Bool)

Returns an initialized output stream for writing to a specified URL.

