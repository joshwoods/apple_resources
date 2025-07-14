

- AppKit
- NSGlyphInfo
-  init(cgGlyph:for:baseString:) 

Initializer

# init(cgGlyph:for:baseString:)

Creates a glyph info object from the specified glyph identifier and font informaton.

macOS 10.13+

``` source
init?(
    cgGlyph glyph: CGGlyph,
    for font: NSFont,
    baseString string: String
)
```

## Parameters 

`glyph`  

The requested CGGlyph object.

`font`  

The font containing the glyph.

`string`  

A string containing the character represented by the glyph.

## Return Value

A glyph info object for the specified glyph or `nil` if the glyph information is not available.

