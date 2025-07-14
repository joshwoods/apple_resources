

- UIKit
- NSLayoutManager
-  ensureLayout(for:) 

Instance Method

# ensureLayout(for:)

Forces the layout manager to perform layout for the specified text container if it hasn’t already.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func ensureLayout(for container: NSTextContainer)
```

## Parameters 

`container`  

The text container for which layout is performed.

## Discussion

The layout manager reserves the right to perform layout for larger ranges. If noncontiguous layout is disabled, then the affected range is always effectively extended to start at the beginning of the text.

## See Also

### Causing glyph generation and layout

func ensureGlyphs(forCharacterRange: NSRange)

Forces the layout manager to generate glyphs for the specified character range if it hasn’t already.

func ensureGlyphs(forGlyphRange: NSRange)

Forces the layout manager to generate glyphs for the specified glyph range if it hasn’t already.

func ensureLayout(forBoundingRect: CGRect, in: NSTextContainer)

Forces the layout manager to perform layout for the specified area in the specified text container if it hasn’t already.

func ensureLayout(forCharacterRange: NSRange)

Forces the layout manager to perform layout for the specified character range if it hasn’t already.

func ensureLayout(forGlyphRange: NSRange)

Forces the layout manager to perform layout for the specified glyph range if it hasn’t already.

var glyphGenerator: NSGlyphGenerator { get set }

The glyph generator that the layout manager uses.

