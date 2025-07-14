

- Core Text
-  kCTForegroundColorFromContextAttributeName 

Global Variable

# kCTForegroundColorFromContextAttributeName

Sets a foreground color using the context’s fill color.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTForegroundColorFromContextAttributeName: CFString
```

## Discussion

Value must be a doc://com.apple.documentation/documentation/corefoundation/cfboolean-s0p object. Default is kCFBooleanFalse. The reason this exists is because an NSAttributedString object defaults to a black color if no color attribute is set. This forces Core Text to set the color in the context. This attribute allows developers to sidestep this, making Core Text set nothing but font information in the CGContext. If set, this attribute also determines the color used by kCTUnderlineStyleAttributeName, in which case it overrides the foreground color.

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

