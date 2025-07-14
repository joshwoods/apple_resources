

- AppKit
- NSLayoutManager
-  invalidateDisplay(forGlyphRange:) 

Instance Method

# invalidateDisplay(forGlyphRange:)

Invalidates a range of glyphs, requiring new layout information, and updates the appropriate regions of any text views that display those glyphs.

macOS 10.7+

``` source
func invalidateDisplay(forGlyphRange glyphRange: NSRange)
```

## Parameters 

`glyphRange`  

The range of glyphs to invalidate.

## Discussion

You should rarely need to invoke this method.

## See Also

### Invalidating glyphs and layout

func invalidateDisplay(forCharacterRange: NSRange)

Invalidates display for the specified character range.

func invalidateGlyphs(forCharacterRange: NSRange, changeInLength: Int, actualCharacterRange: NSRangePointer?)

Invalidates and adjusts the glyphs in the specified character range.

func invalidateLayout(forCharacterRange: NSRange, actualCharacterRange: NSRangePointer?)

Invalidates the layout information for the glyphs that map to the specified character range.

func processEditing(for: NSTextStorage, edited: NSTextStorageEditActions, range: NSRange, changeInLength: Int, invalidatedRange: NSRange)

Notifies the layout manager when an edit action changes the contents of its text storage object.

