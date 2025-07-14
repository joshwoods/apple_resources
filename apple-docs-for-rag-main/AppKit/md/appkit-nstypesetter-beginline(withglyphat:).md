

- AppKit
- NSTypesetter
-  beginLine(withGlyphAt:) 

Instance Method

# beginLine(withGlyphAt:)

Sets up layout parameters at the beginning of a line during typesetting.

macOS

``` source
func beginLine(withGlyphAt glyphIndex: Int)
```

## Parameters 

`glyphIndex`  

The index of the first glyph to be laid out in the line.

## Discussion

Concrete subclass implementations of layoutParagraph(at:) should invoke this method at the beginning of each line.

## See Also

### Laying out a paragraph

func layoutParagraph(at: NSPointPointer) -> Int

Lays out glyphs in the current glyph range until the next paragraph separator is reached.

func beginParagraph()

Sets up layout parameters at the beginning of a paragraph.

func endParagraph()

Sets up layout parameters at the end of a paragraph.

func endLine(withGlyphRange: NSRange)

Sets up layout parameters at the end of a line during typesetting.

