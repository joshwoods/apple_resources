

- Core Text
-  kCTStrokeWidthAttributeName 

Global Variable

# kCTStrokeWidthAttributeName

The stroke width.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTStrokeWidthAttributeName: CFString
```

## Discussion

Value must be a CFNumber object. Default value is `0.0`, or no stroke. This attribute, interpreted as a percentage of font point size, controls the text drawing mode: positive values effect drawing with stroke only; negative values are for stroke and fill. A typical value for outlined text is `3.0`.

## See Also

### Constants

let kCTCharacterShapeAttributeName: CFString

Controls glyph selection.

Deprecated

let kCTFontAttributeName: CFString

The font of the text to which this attribute applies.

let kCTKernAttributeName: CFString

The amount to kern the next character.

let kCTLigatureAttributeName: CFString

The type of ligatures to use.

let kCTForegroundColorAttributeName: CFString

The foreground color of the text to which this attribute applies.

let kCTForegroundColorFromContextAttributeName: CFString

Sets a foreground color using the context’s fill color.

let kCTParagraphStyleAttributeName: CFString

The paragraph style of the text to which this attribute applies.

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

