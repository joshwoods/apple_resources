

- Foundation
- NSString
-  getBytes(\_:maxLength:usedLength:encoding:options:range:remaining:) 

Instance Method

# getBytes(\_:maxLength:usedLength:encoding:options:range:remaining:)

Gets a given range of characters as bytes in a specified encoding.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getBytes(
    _ buffer: UnsafeMutableRawPointer?,
    maxLength maxBufferCount: Int,
    usedLength usedBufferCount: UnsafeMutablePointer?,
    encoding: UInt,
    options: NSString.EncodingConversionOptions = [],
    range: NSRange,
    remaining leftover: NSRangePointer?
) -> Bool
```

## Parameters 

`buffer`  

A buffer into which to store the bytes from the receiver. The returned bytes are *not* `NULL`-terminated.

`maxBufferCount`  

The maximum number of bytes to write to `buffer`.

`usedBufferCount`  

The number of bytes used from `buffer`. Pass `NULL` if you do not need this value.

`encoding`  

The encoding to use for the returned bytes. For possible values, see NSStringEncoding.

`options`  

A mask to specify options to use for converting the receiver’s contents to `encoding` (if conversion is necessary).

`range`  

The range of characters in the receiver to get.

`leftover`  

The remaining range. Pass `NULL` If you do not need this value.

## Return Value

true if some characters were converted, otherwise false.

## Discussion

Conversion might stop when the buffer fills, but it might also stop when the conversion isn’t possible due to the chosen encoding.

## See Also

### Getting Characters and Bytes

func character(at: Int) -> unichar

Returns the character at a given UTF-16 code unit index.

func getCharacters(UnsafeMutablePointer&lt;unichar>, range: NSRange)

Copies characters from a given range in the receiver into a given buffer.

