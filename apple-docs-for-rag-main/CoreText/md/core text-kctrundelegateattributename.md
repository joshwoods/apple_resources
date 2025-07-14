

- Core Text
-  kCTRunDelegateAttributeName 

Global Variable

# kCTRunDelegateAttributeName

The run-delegate object to apply to an attribute range of the string.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTRunDelegateAttributeName: CFString
```

## Discussion

The value must be a CTRunDelegate object. The run delegate controls such typographic traits as glyph ascent, descent, and width. The values returned by the embedded run delegate apply to each glyph resulting from the text in that range. Because an embedded object is only a display-time modification, you should avoid applying this attribute to a range of text with complex behavior, such as text having a change of writing direction or having combining marks. It is thus recommended you apply this attribute to a range containing the single character U+FFFC.

## See Also

### Related Documentation

class CTRunDelegate

A run delegate.

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

let kCTBaselineOffsetAttributeName: CFString

Vertical offset for text position.

