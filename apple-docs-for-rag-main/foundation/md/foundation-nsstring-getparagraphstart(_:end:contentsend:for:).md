

- Foundation
- NSString
-  getParagraphStart(\_:end:contentsEnd:for:) 

Instance Method

# getParagraphStart(\_:end:contentsEnd:for:)

Returns by reference the beginning of the first paragraph and the end of the last paragraph touched by the given range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getParagraphStart(
    _ startPtr: UnsafeMutablePointer?,
    end parEndPtr: UnsafeMutablePointer?,
    contentsEnd contentsEndPtr: UnsafeMutablePointer?,
    for range: NSRange
)
```

## Parameters 

`startPtr`  

Upon return, contains the index of the first character of the paragraph containing the beginning of `aRange`. Pass `NULL` if you do not need this value (in which case the work to compute the value isn’t performed).

`parEndPtr`  

Upon return, contains the index of the first character past the terminator of the paragraph containing the end of `aRange`. Pass `NULL` if you do not need this value (in which case the work to compute the value isn’t performed).

`contentsEndPtr`  

Upon return, contains the index of the first character of the terminator of the paragraph containing the end of `aRange`. Pass `NULL` if you do not need this value (in which case the work to compute the value isn’t performed).

`range`  

A range within the receiver. The value must not exceed the bounds of the receiver.

## Discussion

A paragraph is any segment of text delimited by a carriage return (`U+000D`), newline (`U+000A`), or paragraph separator (`U+2029`).

If `aRange` is contained with a single paragraph, of course, the returned indexes all belong to that paragraph. Similar to getLineStart(_:end:contentsEnd:for:), you can use the results of this method to construct the ranges for paragraphs.

## See Also

### Determining Line and Paragraph Ranges

func getLineStart(UnsafeMutablePointer&lt;Int>?, end: UnsafeMutablePointer&lt;Int>?, contentsEnd: UnsafeMutablePointer&lt;Int>?, for: NSRange)

Returns by reference the beginning of the first line and the end of the last line touched by the given range.

func lineRange(for: NSRange) -> NSRange

Returns the range of characters representing the line or lines containing a given range.

func paragraphRange(for: NSRange) -> NSRange

Returns the range of characters representing the paragraph or paragraphs containing a given range.

