

- AppKit
- NSText
-  replaceCharacters(in:with:) 

Instance Method

# replaceCharacters(in:with:)

Replaces the characters in the given range with those in the given string.

macOS

``` source
@MainActor
func replaceCharacters(
    in range: NSRange,
    with string: String
)
```

## Parameters 

`range`  

The range of characters to be replaced.

`string`  

The replacement string.

## Discussion

For a rich text object, the text of `aString` is assigned the formatting attributes of the first character of the text it replaces, or of the character immediately before `aRange` if the range’s length is 0. If the range’s location is 0, the formatting attributes of the first character in the receiver are used.

This method does not include undo support by default. Clients must invoke shouldChangeText(inRanges:replacementStrings:) or shouldChangeText(in:replacementString:) to include this method in an undoable action.

In most cases, programmatic modification of the text is best done by operating on the text storage directly, using the general methods of NSMutableAttributedString.

## See Also

### Replacing text

func replaceCharacters(in: NSRange, withRTF: Data)

Replaces the characters in the given range with RTF text interpreted from the given RTF data.

func replaceCharacters(in: NSRange, withRTFD: Data)

Replaces the characters in the given range with RTFD text interpreted from the given RTFD data.

