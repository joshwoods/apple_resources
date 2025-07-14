

- AppKit
- NSATSTypesetter
-  attributedString 

Instance Property

# attributedString

The backing store that contains the text on which this typesetter operates.

macOS

``` source
unowned(unsafe) var attributedString: NSAttributedString? { get set }
```

## See Also

### Accessing paragraph information

func setParagraphGlyphRange(NSRange, separatorGlyphRange: NSRange)

Sets the glyph range being processed and the paragraph separator glyph range (the range of the paragraph separator character or characters).

var paragraphGlyphRange: NSRange

The current glyph range being processed.

var paragraphSeparatorGlyphRange: NSRange

The current paragraph separator range that contains the current glyph range and extends from one paragraph separator character to the next.

