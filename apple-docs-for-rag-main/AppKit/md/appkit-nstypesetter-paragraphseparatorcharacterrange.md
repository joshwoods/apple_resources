

- AppKit
- NSTypesetter
-  paragraphSeparatorCharacterRange 

Instance Property

# paragraphSeparatorCharacterRange

Returns the current paragraph separator character range.

macOS

``` source
var paragraphSeparatorCharacterRange: NSRange { get }
```

## Return Value

The current paragraph separator character range, which is the full range that contains the current character range and that extends from one paragraph separator character to the next.

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

var paragraphSeparatorGlyphRange: NSRange

Returns the current paragraph separator range.

var paragraphCharacterRange: NSRange

Returns the character range currently being processed.

var attributesForExtraLineFragment: [NSAttributedString.Key : Any]

Returns the attributes used to lay out the extra line fragment.

