

- Foundation
- NSAttributedString
-  doubleClick(at:) 

Instance Method

# doubleClick(at:)

Returns the range of characters that form a word (or other linguistic unit) surrounding the specified index, taking language characteristics into account.

macOS 10.0+

``` source
func doubleClick(at location: Int) -> NSRange
```

## Parameters 

`location`  

The index in the attributed string.

## Return Value

Returns the range of characters that form a word (or other linguistic unit) surrounding the given index, taking language characteristics into account.

## Discussion

Raises an rangeException if `index` lies beyond the end of the receiver’s characters.

## See Also

### Calculating linguistic units

func lineBreak(before: Int, within: NSRange) -> Int

Returns the appropriate line break when the character at the index doesn’t fit on the same line as the character at the beginning of the range.

func lineBreakByHyphenating(before: Int, within: NSRange) -> Int

Returns the index of the closest character before the specified index, and within the specified range, that can fit on a new line by hyphenating.

func nextWord(from: Int, forward: Bool) -> Int

Returns the index of the first character of the word after or before the specified index.

