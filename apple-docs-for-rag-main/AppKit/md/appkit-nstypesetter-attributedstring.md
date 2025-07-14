

- AppKit
- NSTypesetter
-  attributedString 

Instance Property

# attributedString

Returns the text backing store, usually an instance of `NSTextStorage`.

macOS

``` source
unowned(unsafe) var attributedString: NSAttributedString? { get set }
```

## Return Value

The text backing store.

## See Also

### Accessing paragraph typesetting information

var currentParagraphStyle: NSParagraphStyle?

Returns the paragraph style object for the text being typeset.

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

