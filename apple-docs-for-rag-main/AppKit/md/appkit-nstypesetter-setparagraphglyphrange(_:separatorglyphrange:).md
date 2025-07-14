

- AppKit
- NSTypesetter
-  setParagraphGlyphRange(\_:separatorGlyphRange:) 

Instance Method

# setParagraphGlyphRange(\_:separatorGlyphRange:)

Sets the current glyph range being processed.

macOS

``` source
func setParagraphGlyphRange(
    _ paragraphRange: NSRange,
    separatorGlyphRange paragraphSeparatorRange: NSRange
)
```

## Parameters 

`paragraphRange`  

The current glyph range being processed.

`paragraphSeparatorRange`  

The range of the paragraph separator character or characters.

## See Also

### Accessing paragraph typesetting information

var currentParagraphStyle: NSParagraphStyle?

Returns the paragraph style object for the text being typeset.

var attributedString: NSAttributedString?

Returns the text backing store, usually an instance of `NSTextStorage`.

var paragraphGlyphRange: NSRange

Returns the glyph range currently being processed.

var paragraphSeparatorGlyphRange: NSRange

Returns the current paragraph separator range.

var paragraphCharacterRange: NSRange

Returns the character range currently being processed.

var paragraphSeparatorCharacterRange: NSRange

Returns the current paragraph separator character range.

var attributesForExtraLineFragment: [NSAttributedString.Key : Any]

Returns the attributes used to lay out the extra line fragment.

