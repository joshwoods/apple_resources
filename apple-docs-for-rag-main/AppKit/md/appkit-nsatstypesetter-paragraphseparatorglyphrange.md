

- AppKit
- NSATSTypesetter
-  paragraphSeparatorGlyphRange 

Instance Property

# paragraphSeparatorGlyphRange

The current paragraph separator range that contains the current glyph range and extends from one paragraph separator character to the next.

macOS

``` source
var paragraphSeparatorGlyphRange: NSRange { get }
```

## See Also

### Accessing paragraph information

var attributedString: NSAttributedString?

The backing store that contains the text on which this typesetter operates.

func setParagraphGlyphRange(NSRange, separatorGlyphRange: NSRange)

Sets the glyph range being processed and the paragraph separator glyph range (the range of the paragraph separator character or characters).

var paragraphGlyphRange: NSRange

The current glyph range being processed.

