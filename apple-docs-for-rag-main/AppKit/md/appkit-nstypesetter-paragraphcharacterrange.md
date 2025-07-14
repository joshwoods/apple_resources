

- AppKit
- NSTypesetter
-  paragraphCharacterRange 

Instance Property

# paragraphCharacterRange

Returns the character range currently being processed.

macOS

``` source
var paragraphCharacterRange: NSRange { get }
```

## Return Value

The character range currently being processed.

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

var paragraphSeparatorCharacterRange: NSRange

Returns the current paragraph separator character range.

var attributesForExtraLineFragment: [NSAttributedString.Key : Any]

Returns the attributes used to lay out the extra line fragment.

