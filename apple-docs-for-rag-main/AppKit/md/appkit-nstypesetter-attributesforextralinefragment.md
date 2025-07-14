

- AppKit
- NSTypesetter
-  attributesForExtraLineFragment 

Instance Property

# attributesForExtraLineFragment

Returns the attributes used to lay out the extra line fragment.

macOS

``` source
var attributesForExtraLineFragment: [NSAttributedString.Key : Any] { get }
```

## Return Value

A dictionary of attributes used to lay out the extra line fragment.

## Discussion

The default implementation tries to use the `NSTextView` method typingAttributes if possible; otherwise, it uses the attributes for the last character.

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

var paragraphSeparatorCharacterRange: NSRange

Returns the current paragraph separator character range.

