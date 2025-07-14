

- AppKit
- NSLayoutManager
-  ensureGlyphs(forCharacterRange:) 

Instance Method

# ensureGlyphs(forCharacterRange:)

Forces the layout manager to generate glyphs for the specified character range if it hasn’t already.

macOS 10.7+

``` source
func ensureGlyphs(forCharacterRange charRange: NSRange)
```

## Parameters 

`charRange`  

The character range for which glyphs are generated.

## Discussion

The layout manager reserves the right to perform glyph generation for larger ranges. If noncontiguous layout is disabled, then the affected range is always effectively extended to start at the beginning of the text.

## See Also

### Causing glyph generation and layout

func ensureGlyphs(forGlyphRange: NSRange)

Forces the layout manager to generate glyphs for the specified glyph range if it hasn’t already.

func ensureLayout(forBoundingRect: NSRect, in: NSTextContainer)

Forces the layout manager to perform layout for the specified area in the specified text container if it hasn’t already.

func ensureLayout(forCharacterRange: NSRange)

Forces the layout manager to perform layout for the specified character range if it hasn’t already.

func ensureLayout(forGlyphRange: NSRange)

Forces the layout manager to perform layout for the specified glyph range if it hasn’t already.

func ensureLayout(for: NSTextContainer)

Forces the layout manager to perform layout for the specified text container if it hasn’t already.

var glyphGenerator: NSGlyphGenerator

The glyph generator that the layout manager uses.

