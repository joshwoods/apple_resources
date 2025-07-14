

- Core Text
-  kCTKernAttributeName 

Global Variable

# kCTKernAttributeName

The amount to kern the next character.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTKernAttributeName: CFString
```

## Discussion

The value associated with this attribute must be a CFNumber float. Default is standard kerning. The kerning attribute indicates how many points the following character should be shifted from its default offset as defined by the current character’s font in points: a positive kern indicates a shift farther away from and a negative kern indicates a shift closer to the current character. If this attribute is not present, standard kerning is used. If this attribute is set to `0.0`, no kerning is done at all.

## See Also

### Constants

let kCTCharacterShapeAttributeName: CFString

Controls glyph selection.

Deprecated

let kCTFontAttributeName: CFString

The font of the text to which this attribute applies.

let kCTLigatureAttributeName: CFString

The type of ligatures to use.

let kCTForegroundColorAttributeName: CFString

The foreground color of the text to which this attribute applies.

let kCTForegroundColorFromContextAttributeName: CFString

Sets a foreground color using the context’s fill color.

let kCTParagraphStyleAttributeName: CFString

The paragraph style of the text to which this attribute applies.

let kCTStrokeWidthAttributeName: CFString

The stroke width.

let kCTStrokeColorAttributeName: CFString

The stroke color.

let kCTSuperscriptAttributeName: CFString

Controls vertical text positioning.

let kCTUnderlineColorAttributeName: CFString

The underline color.

let kCTUnderlineStyleAttributeName: CFString

The style of underlining, to be applied at render time, for the text to which this attribute applies.

let kCTVerticalFormsAttributeName: CFString

The orientation of the glyphs in the text to which this attribute applies.

let kCTGlyphInfoAttributeName: CFString

The glyph info object to apply to the text associated with this attribute.

let kCTRunDelegateAttributeName: CFString

The run-delegate object to apply to an attribute range of the string.

let kCTBaselineOffsetAttributeName: CFString

Vertical offset for text position.

