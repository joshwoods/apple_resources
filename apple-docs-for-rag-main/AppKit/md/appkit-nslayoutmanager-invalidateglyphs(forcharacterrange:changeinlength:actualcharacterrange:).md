

- AppKit
- NSLayoutManager
-  invalidateGlyphs(forCharacterRange:changeInLength:actualCharacterRange:) 

Instance Method

# invalidateGlyphs(forCharacterRange:changeInLength:actualCharacterRange:)

Invalidates and adjusts the glyphs in the specified character range.

macOS 10.7+

``` source
func invalidateGlyphs(
    forCharacterRange charRange: NSRange,
    changeInLength delta: Int,
    actualCharacterRange actualCharRange: NSRangePointer?
)
```

## Parameters 

`charRange`  

The range of characters for which to invalidate glyphs.

`delta`  

The number of characters added or removed.

`actualCharRange`  

If not `NULL`, on output, the actual range invalidated after any necessary expansion. This range can be larger than the range of characters given due to the effect of context on glyphs and layout.

## Discussion

This method invalidates the cached glyphs for the characters in the given character range, adjusts the character indices of all the subsequent glyphs by the change in length, and invalidates the new character range. This method invalidates only glyph information and performs no glyph generation or layout. Because invalidating glyphs also invalidates layout, after invoking this method you should also invoke invalidateLayout(forCharacterRange:actualCharacterRange:), passing `charRange` as the first argument.

This method is used by the layout mechanism and should be invoked only during typesetting, in almost all cases only by the typesetter. For example, a custom typesetter might invoke it.

## See Also

### Invalidating glyphs and layout

func invalidateDisplay(forCharacterRange: NSRange)

Invalidates display for the specified character range.

func invalidateDisplay(forGlyphRange: NSRange)

Invalidates a range of glyphs, requiring new layout information, and updates the appropriate regions of any text views that display those glyphs.

func invalidateLayout(forCharacterRange: NSRange, actualCharacterRange: NSRangePointer?)

Invalidates the layout information for the glyphs that map to the specified character range.

func processEditing(for: NSTextStorage, edited: NSTextStorageEditActions, range: NSRange, changeInLength: Int, invalidatedRange: NSRange)

Notifies the layout manager when an edit action changes the contents of its text storage object.

