

- Foundation
- NSString
-  lineRange(for:) 

Instance Method

# lineRange(for:)

Returns the range of characters representing the line or lines containing a given range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func lineRange(for range: NSRange) -> NSRange
```

## Parameters 

`range`  

A range within the receiver. The value must not exceed the bounds of the receiver.

## Return Value

The range of characters representing the line or lines containing `aRange`, including the line termination characters. See getLineStart(_:end:contentsEnd:for:) for a discussion of line terminators.

## See Also

### Related Documentation

func substring(with: NSRange) -> String

Returns a string object containing the characters of the receiver that lie within a given range.

### Determining Line and Paragraph Ranges

func getLineStart(UnsafeMutablePointer&lt;Int>?, end: UnsafeMutablePointer&lt;Int>?, contentsEnd: UnsafeMutablePointer&lt;Int>?, for: NSRange)

Returns by reference the beginning of the first line and the end of the last line touched by the given range.

func getParagraphStart(UnsafeMutablePointer&lt;Int>?, end: UnsafeMutablePointer&lt;Int>?, contentsEnd: UnsafeMutablePointer&lt;Int>?, for: NSRange)

Returns by reference the beginning of the first paragraph and the end of the last paragraph touched by the given range.

func paragraphRange(for: NSRange) -> NSRange

Returns the range of characters representing the paragraph or paragraphs containing a given range.

