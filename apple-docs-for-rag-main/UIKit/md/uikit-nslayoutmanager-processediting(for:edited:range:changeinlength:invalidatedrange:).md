

- UIKit
- NSLayoutManager
-  processEditing(for:edited:range:changeInLength:invalidatedRange:) 

Instance Method

# processEditing(for:edited:range:changeInLength:invalidatedRange:)

Notifies the layout manager when an edit action changes the contents of its text storage object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func processEditing(
    for textStorage: NSTextStorage,
    edited editMask: NSTextStorage.EditActions,
    range newCharRange: NSRange,
    changeInLength delta: Int,
    invalidatedRange invalidatedCharRange: NSRange
)
```

## Parameters 

`textStorage`  

The text storage object processing edits.

`editMask`  

The types of edits done: `NSTextStorageEditedAttributes`, `NSTextStorageEditedCharacters`, or both.

`newCharRange`  

The range in the final string that was explicitly edited.

`delta`  

The length delta for the editing changes.

`invalidatedCharRange`  

The range of characters that changed as a result of attribute fixing. This invalidated range is either equal to `newCharRange` or larger.

## Discussion

The processEditing() method of NSTextStorage calls this method to notify the layout manager of an edit action. Layout managers must not change the contents of the text storage during the execution of this message.

## See Also

### Invalidating glyphs and layout

func invalidateDisplay(forCharacterRange: NSRange)

Invalidates display for the specified character range.

func invalidateDisplay(forGlyphRange: NSRange)

Invalidates a range of glyphs, requiring new layout information, and updates the appropriate regions of any text views that display those glyphs.

func invalidateGlyphs(forCharacterRange: NSRange, changeInLength: Int, actualCharacterRange: NSRangePointer?)

Invalidates and adjusts the glyphs in the specified character range.

func invalidateLayout(forCharacterRange: NSRange, actualCharacterRange: NSRangePointer?)

Invalidates the layout information for the glyphs that map to the specified character range.

