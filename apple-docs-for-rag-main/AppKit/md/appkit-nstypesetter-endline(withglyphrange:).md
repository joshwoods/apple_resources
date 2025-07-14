

- AppKit
- NSTypesetter
-  endLine(withGlyphRange:) 

Instance Method

# endLine(withGlyphRange:)

Sets up layout parameters at the end of a line during typesetting.

macOS

``` source
func endLine(withGlyphRange lineGlyphRange: NSRange)
```

## Parameters 

`lineGlyphRange`  

The range of glyphs laid out in the line.

## Discussion

Concrete subclass implementations of layoutParagraph(at:) should invoke this method at the end of each line.

## See Also

### Laying out a paragraph

func layoutParagraph(at: NSPointPointer) -> Int

Lays out glyphs in the current glyph range until the next paragraph separator is reached.

func beginParagraph()

Sets up layout parameters at the beginning of a paragraph.

func endParagraph()

Sets up layout parameters at the end of a paragraph.

func beginLine(withGlyphAt: Int)

Sets up layout parameters at the beginning of a line during typesetting.

