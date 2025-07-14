

- AppKit
- NSLayoutManager
-  invalidateLayout(forCharacterRange:actualCharacterRange:) 

Instance Method

# invalidateLayout(forCharacterRange:actualCharacterRange:)

Invalidates the layout information for the glyphs that map to the specified character range.

macOS 10.5+

``` source
func invalidateLayout(
    forCharacterRange charRange: NSRange,
    actualCharacterRange actualCharRange: NSRangePointer?
)
```

## Parameters 

`charRange`  

The range of characters to invalidate.

`actualCharRange`  

If not `NULL`, on output, the actual range invalidated after any necessary expansion.

## Discussion

This method has the same effect as invalidateLayout(forCharacterRange:isSoft:actualCharacterRange:) with `flag` set to false.

This method only invalidates information; it performs no glyph generation or layout. You should rarely need to invoke this method.

## See Also

### Invalidating glyphs and layout

func invalidateDisplay(forCharacterRange: NSRange)

Invalidates display for the specified character range.

func invalidateDisplay(forGlyphRange: NSRange)

Invalidates a range of glyphs, requiring new layout information, and updates the appropriate regions of any text views that display those glyphs.

func invalidateGlyphs(forCharacterRange: NSRange, changeInLength: Int, actualCharacterRange: NSRangePointer?)

Invalidates and adjusts the glyphs in the specified character range.

func processEditing(for: NSTextStorage, edited: NSTextStorageEditActions, range: NSRange, changeInLength: Int, invalidatedRange: NSRange)

Notifies the layout manager when an edit action changes the contents of its text storage object.

