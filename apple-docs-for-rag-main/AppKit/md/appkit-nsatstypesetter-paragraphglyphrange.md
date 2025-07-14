

- AppKit
- NSATSTypesetter
-  paragraphGlyphRange 

Instance Property

# paragraphGlyphRange

The current glyph range being processed.

macOS

``` source
var paragraphGlyphRange: NSRange { get }
```

## See Also

### Accessing paragraph information

var attributedString: NSAttributedString?

The backing store that contains the text on which this typesetter operates.

func setParagraphGlyphRange(NSRange, separatorGlyphRange: NSRange)

Sets the glyph range being processed and the paragraph separator glyph range (the range of the paragraph separator character or characters).

var paragraphSeparatorGlyphRange: NSRange

The current paragraph separator range that contains the current glyph range and extends from one paragraph separator character to the next.

