

- AppKit
- NSTypesetter
-  paragraphSeparatorGlyphRange 

Instance Property

# paragraphSeparatorGlyphRange

Returns the current paragraph separator range.

macOS

``` source
var paragraphSeparatorGlyphRange: NSRange { get }
```

## Return Value

The current paragraph separator range, which is the full range that contains the current glyph range and that extends from one paragraph separator character to the next.

## See Also

### Accessing paragraph typesetting information

var currentParagraphStyle: NSParagraphStyle?

Returns the paragraph style object for the text being typeset.

var attributedString: NSAttributedString?

Returns the text backing store, usually an instance of `NSTextStorage`.

func setParagraphGlyphRange(NSRange, separatorGlyphRange: NSRange)

Sets the current glyph range being processed.

var paragraphGlyphRange: NSRange

Returns the glyph range currently being processed.

var paragraphCharacterRange: NSRange

Returns the character range currently being processed.

var paragraphSeparatorCharacterRange: NSRange

Returns the current paragraph separator character range.

var attributesForExtraLineFragment: [NSAttributedString.Key : Any]

Returns the attributes used to lay out the extra line fragment.

