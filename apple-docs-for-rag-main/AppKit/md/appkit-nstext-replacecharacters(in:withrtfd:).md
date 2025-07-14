

- AppKit
- NSText
-  replaceCharacters(in:withRTFD:) 

Instance Method

# replaceCharacters(in:withRTFD:)

Replaces the characters in the given range with RTFD text interpreted from the given RTFD data.

macOS

``` source
@MainActor
func replaceCharacters(
    in range: NSRange,
    withRTFD rtfdData: Data
)
```

## Parameters 

`range`  

The range of characters to be replaced.

`rtfdData`  

The RTFD data from which to derive the replacement string.

## Discussion

This method applies only to rich text objects.

This method does not include undo support by default. Clients must invoke shouldChangeText(inRanges:replacementStrings:) or shouldChangeText(in:replacementString:) to include this method in an undoable action.

This method is designed for transferring text from out-of-process sources such as the pasteboard. In most cases, programmatic modification of the text is best done by operating on the text storage directly, using the general methods of NSMutableAttributedString.

## See Also

### Replacing text

func replaceCharacters(in: NSRange, withRTF: Data)

Replaces the characters in the given range with RTF text interpreted from the given RTF data.

func replaceCharacters(in: NSRange, with: String)

Replaces the characters in the given range with those in the given string.

