

- Foundation
- NSAttributedString
-  lineBreakByHyphenating(before:within:) 

Instance Method

# lineBreakByHyphenating(before:within:)

Returns the index of the closest character before the specified index, and within the specified range, that can fit on a new line by hyphenating.

macOS 10.0+

``` source
func lineBreakByHyphenating(
    before location: Int,
    within aRange: NSRange
) -> Int
```

## Parameters 

`location`  

The location in the attributed string.

`aRange`  

The range.

## Return Value

Returns the index of the closest character before `index` within `aRange`, that can be placed on a new line by hyphenating. Returns `NSNotFound` if no line break by hyphenation is possible before `index`.

## Discussion

In other words, during text layout, finds the appropriate line break by hyphenation (the character index at which the hyphen glyph should be inserted) when the character at `index` won’t fit on the same line as the character at the beginning of `aRange`.

Raises an rangeException if `index` or any part of `aRange` lies beyond the end of the receiver’s characters.

## See Also

### Calculating linguistic units

func doubleClick(at: Int) -> NSRange

Returns the range of characters that form a word (or other linguistic unit) surrounding the specified index, taking language characteristics into account.

func lineBreak(before: Int, within: NSRange) -> Int

Returns the appropriate line break when the character at the index doesn’t fit on the same line as the character at the beginning of the range.

func nextWord(from: Int, forward: Bool) -> Int

Returns the index of the first character of the word after or before the specified index.

