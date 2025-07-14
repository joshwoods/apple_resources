

- Foundation
- NSString
-  character(at:) 

Instance Method

# character(at:)

Returns the character at a given UTF-16 code unit index.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func character(at index: Int) -> unichar
```

## Parameters 

`index`  

The index of the character to retrieve.

Important

Raises an `NSRangeException` if `index` lies beyond the end of the receiver.

## Return Value

The character at the array position given by `index`.

## Discussion

You should always use the rangeOfComposedCharacterSequence(at:) or rangeOfComposedCharacterSequences(for:) method to determine character boundaries, so that any surrogate pairs or character clusters are handled correctly.

## See Also

### Getting Characters and Bytes

func getCharacters(UnsafeMutablePointer&lt;unichar>, range: NSRange)

Copies characters from a given range in the receiver into a given buffer.

func getBytes(UnsafeMutableRawPointer?, maxLength: Int, usedLength: UnsafeMutablePointer&lt;Int>?, encoding: UInt, options: NSString.EncodingConversionOptions, range: NSRange, remaining: NSRangePointer?) -> Bool

Gets a given range of characters as bytes in a specified encoding.

