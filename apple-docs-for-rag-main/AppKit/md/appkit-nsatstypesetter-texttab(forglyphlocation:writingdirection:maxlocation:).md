

- AppKit
- NSATSTypesetter
-  textTab(forGlyphLocation:writingDirection:maxLocation:) 

Instance Method

# textTab(forGlyphLocation:writingDirection:maxLocation:)

Returns the text tab closest to the specified glyph location and not beyond a maximum position.

macOS

``` source
func textTab(
    forGlyphLocation glyphLocation: CGFloat,
    writingDirection direction: NSWritingDirection,
    maxLocation: CGFloat
) -> NSTextTab?
```

## Discussion

The typesetter calls this method whenever it finds a tab character. To determine the width to advance the next glyph, the typesetter examines the NSParagraphStyle tab array and the default tab interval.

