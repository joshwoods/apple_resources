

- AppKit
- NSTypesetter
-  endParagraph() 

Instance Method

# endParagraph()

Sets up layout parameters at the end of a paragraph.

macOS

``` source
func endParagraph()
```

## Discussion

Concrete subclasses should invoke this method at the end of their layoutParagraph(at:) implementation.

## See Also

### Laying out a paragraph

func layoutParagraph(at: NSPointPointer) -> Int

Lays out glyphs in the current glyph range until the next paragraph separator is reached.

func beginParagraph()

Sets up layout parameters at the beginning of a paragraph.

func beginLine(withGlyphAt: Int)

Sets up layout parameters at the beginning of a line during typesetting.

func endLine(withGlyphRange: NSRange)

Sets up layout parameters at the end of a line during typesetting.

