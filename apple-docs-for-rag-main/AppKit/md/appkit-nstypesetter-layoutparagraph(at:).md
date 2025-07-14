

- AppKit
- NSTypesetter
-  layoutParagraph(at:) 

Instance Method

# layoutParagraph(at:)

Lays out glyphs in the current glyph range until the next paragraph separator is reached.

macOS

``` source
func layoutParagraph(at lineFragmentOrigin: NSPointPointer) -> Int
```

## Parameters 

`lineFragmentOrigin`  

The upper-left corner of line fragment rectangle. On return, `lineFragmentOrigin` contains the next origin.

## Return Value

The next glyph index; usually the index right after the paragraph separator, but it can be inside the paragraph range if, for example, the end of the text container is reached before the paragraph separator.

## Discussion

Concrete subclasses must implement this method. A concrete implementation must invoke beginParagraph(), beginLine(withGlyphAt:), endLine(withGlyphRange:), and endParagraph().

## See Also

### Laying out a paragraph

func beginParagraph()

Sets up layout parameters at the beginning of a paragraph.

func endParagraph()

Sets up layout parameters at the end of a paragraph.

func beginLine(withGlyphAt: Int)

Sets up layout parameters at the beginning of a line during typesetting.

func endLine(withGlyphRange: NSRange)

Sets up layout parameters at the end of a line during typesetting.

