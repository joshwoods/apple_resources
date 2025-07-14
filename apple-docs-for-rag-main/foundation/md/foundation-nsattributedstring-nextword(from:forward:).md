

- Foundation
- NSAttributedString
-  nextWord(from:forward:) 

Instance Method

# nextWord(from:forward:)

Returns the index of the first character of the word after or before the specified index.

macOS 10.0+

``` source
func nextWord(
    from location: Int,
    forward isForward: Bool
) -> Int
```

## Parameters 

`location`  

The index in the attribute string.

`isForward`  

true if the search should be forward, otherwise false.

## Return Value

true if this is the first character after `index` that begins a word; if `flag` is false, it’s the first character before `index` that begins a word, whether `index` is located within a word or not.

## Discussion

If `index` lies at either end of the string and the search direction would progress past that end, it’s returned unchanged.

This method is intended for moving the insertion point during editing, not for linguistic analysis or parsing of text.

Raises an rangeException if `index` lies beyond the end of the receiver’s characters.

## See Also

### Calculating linguistic units

func doubleClick(at: Int) -> NSRange

Returns the range of characters that form a word (or other linguistic unit) surrounding the specified index, taking language characteristics into account.

func lineBreak(before: Int, within: NSRange) -> Int

Returns the appropriate line break when the character at the index doesn’t fit on the same line as the character at the beginning of the range.

func lineBreakByHyphenating(before: Int, within: NSRange) -> Int

Returns the index of the closest character before the specified index, and within the specified range, that can fit on a new line by hyphenating.

