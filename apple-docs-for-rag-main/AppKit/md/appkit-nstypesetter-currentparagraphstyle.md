

- AppKit
- NSTypesetter
-  currentParagraphStyle 

Instance Property

# currentParagraphStyle

Returns the paragraph style object for the text being typeset.

macOS

``` source
@NSCopying
var currentParagraphStyle: NSParagraphStyle? { get }
```

## Return Value

The paragraph style object for the text being typeset. This value is valid only while the typesetter is performing layout.

## See Also

### Accessing paragraph typesetting information

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

var paragraphSeparatorCharacterRange: NSRange

Returns the current paragraph separator character range.

var attributesForExtraLineFragment: [NSAttributedString.Key : Any]

Returns the attributes used to lay out the extra line fragment.

