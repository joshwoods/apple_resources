

- Foundation
- NSString
-  getCharacters(\_:range:) 

Instance Method

# getCharacters(\_:range:)

Copies characters from a given range in the receiver into a given buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getCharacters(
    _ buffer: UnsafeMutablePointer,
    range: NSRange
)
```

## Parameters 

`buffer`  

Upon return, contains the characters from the receiver. `buffer` must be large enough to contain the characters in the range `aRange` (`aRange.length*sizeof(unichar)`).

`range`  

The range of characters to retrieve. The range must not exceed the bounds of the receiver.

Important

Raises an `NSRangeException` if any part of `aRange` lies beyond the bounds of the receiver.

## Discussion

This method does not add a `NULL` character.

The abstract implementation of this method uses character(at:) repeatedly, correctly extracting the characters, though very inefficiently. Subclasses should override it to provide a fast implementation.

You should always use the rangeOfComposedCharacterSequence(at:) or rangeOfComposedCharacterSequences(for:) method to determine character boundaries, so that any surrogate pairs or character clusters are handled correctly.

## See Also

### Getting Characters and Bytes

func character(at: Int) -> unichar

Returns the character at a given UTF-16 code unit index.

func getBytes(UnsafeMutableRawPointer?, maxLength: Int, usedLength: UnsafeMutablePointer&lt;Int>?, encoding: UInt, options: NSString.EncodingConversionOptions, range: NSRange, remaining: NSRangePointer?) -> Bool

Gets a given range of characters as bytes in a specified encoding.

