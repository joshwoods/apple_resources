

- AppKit
- NSATSTypesetter
-  setParagraphGlyphRange(\_:separatorGlyphRange:) 

Instance Method

# setParagraphGlyphRange(\_:separatorGlyphRange:)

Sets the glyph range being processed and the paragraph separator glyph range (the range of the paragraph separator character or characters).

macOS

``` source
func setParagraphGlyphRange(
    _ paragraphRange: NSRange,
    separatorGlyphRange paragraphSeparatorRange: NSRange
)
```

## Parameters 

`paragraphRange`  

The glyph range that becomes current.

`paragraphSeparatorRange`  

The paragraph separator glyph range that becomes current.

## See Also

### Accessing paragraph information

var attributedString: NSAttributedString?

The backing store that contains the text on which this typesetter operates.

var paragraphGlyphRange: NSRange

The current glyph range being processed.

var paragraphSeparatorGlyphRange: NSRange

The current paragraph separator range that contains the current glyph range and extends from one paragraph separator character to the next.

