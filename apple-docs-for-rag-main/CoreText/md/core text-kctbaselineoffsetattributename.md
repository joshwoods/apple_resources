

- Core Text
-  kCTBaselineOffsetAttributeName 

Global Variable

# kCTBaselineOffsetAttributeName

Vertical offset for text position.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let kCTBaselineOffsetAttributeName: CFString
```

## Discussion

The value of this attribute must be a CFNumber float. The default is standard positioning, following the baselines of the fonts used.

The baseline offset attribute indicates how many points the characters should be shifted perpendicular to their baseline. For horizontal text, a positive baseline value indicates a shift above the text baseline, and a negative baseline value indicates a shift below the text baseline. For vertical text, a positive baseline value indicates a shift to the right of the text baseline, and a negative baseline value indicates a shift to the left of the text baseline. If this value is set to `0.0`, no baseline shift will be performed.

Important

This attribute is different from baselineOffset. If you are writing code for TextKit, you need to use baselineOffset.

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

