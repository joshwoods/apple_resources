

- Core Text
-  kCTCharacterShapeAttributeName Deprecated

Global Variable

# kCTCharacterShapeAttributeName

Controls glyph selection.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
let kCTCharacterShapeAttributeName: CFString
```

Deprecated

Use feature type kCharacterShapeType with the appropriate selector

## Discussion

Value must be a CFNumber object. Default is value is `0` (disabled). A non-zero value is interpreted as Apple Type Services `kCharacterShapeType` selector `+ 1` (see `` for selectors). For example, an attribute value of `1` corresponds to `kTraditionalCharactersSelector`.

## See Also

### Constants

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

let kCTBaselineOffsetAttributeName: CFString

Vertical offset for text position.

