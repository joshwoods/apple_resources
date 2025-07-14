

- UIKit
- NSLayoutManager
-  invalidateDisplay(forCharacterRange:) 

Instance Method

# invalidateDisplay(forCharacterRange:)

Invalidates display for the specified character range.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func invalidateDisplay(forCharacterRange charRange: NSRange)
```

## Parameters 

`charRange`  

The character range for which display is invalidated.

## Discussion

Parts of the range that are not laid out are remembered and redisplayed later when the layout is available. Does not actually cause layout.

## See Also

### Invalidating glyphs and layout

func invalidateDisplay(forGlyphRange: NSRange)

Invalidates a range of glyphs, requiring new layout information, and updates the appropriate regions of any text views that display those glyphs.

func invalidateGlyphs(forCharacterRange: NSRange, changeInLength: Int, actualCharacterRange: NSRangePointer?)

Invalidates and adjusts the glyphs in the specified character range.

func invalidateLayout(forCharacterRange: NSRange, actualCharacterRange: NSRangePointer?)

Invalidates the layout information for the glyphs that map to the specified character range.

func processEditing(for: NSTextStorage, edited: NSTextStorage.EditActions, range: NSRange, changeInLength: Int, invalidatedRange: NSRange)

Notifies the layout manager when an edit action changes the contents of its text storage object.

