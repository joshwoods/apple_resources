

- Swift
- StringProtocol
-  getBytes(\_:maxLength:usedLength:encoding:options:range:remaining:) 

Instance Method

# getBytes(\_:maxLength:usedLength:encoding:options:range:remaining:)

Writes the given `range` of characters into `buffer` in a given `encoding`, without any allocations. Does not NULL-terminate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getBytes(
    _ buffer: inout [UInt8],
    maxLength maxBufferCount: Int,
    usedLength usedBufferCount: UnsafeMutablePointer,
    encoding: String.Encoding,
    options: String.EncodingConversionOptions = [],
    range: R,
    remaining leftover: UnsafeMutablePointer>
) -> Bool where R : RangeExpression, R.Bound == String.Index
```

## Parameters 

`buffer`  

A buffer into which to store the bytes from the receiver. The returned bytes are not NUL-terminated.

`maxBufferCount`  

The maximum number of bytes to write to buffer.

`usedBufferCount`  

The number of bytes used from buffer. Pass `nil` if you do not need this value.

`encoding`  

The encoding to use for the returned bytes.

`options`  

A mask to specify options to use for converting the receiver’s contents to `encoding` (if conversion is necessary).

`range`  

The range of characters in the receiver to get.

`leftover`  

The remaining range. Pass `nil` If you do not need this value.

## Return Value

`true` if some characters were converted, `false` otherwise.

## Discussion

Note

Conversion stops when the buffer fills or when the conversion isn’t possible due to the chosen encoding.

Note

Will get a maximum of `min(buffer.count, maxLength)` bytes.

