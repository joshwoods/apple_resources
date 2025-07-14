

- Core Text
-  kCTTrackingAttributeName 

Global Variable

# kCTTrackingAttributeName

The tracking for the text.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
let kCTTrackingAttributeName: CFString
```

## Discussion

The value associated with this attribute must be a doc://com.apple.documentation/documentation/corefoundation/cfnumber-rjd float. The default is `0` (no tracking).

Tracking adds space, in points, between the specified character cluster. A positive value increases the spacing between characters, while a negative value brings the characters closer together. For example, setting kCTTrackingAttributeName to 0.1 adds 0.1 point of spacing between each character of the text.

The effect of this attribute is similar to kCTKernAttributeName, but it treats tracking as trailing whitespace and a nonzero amount disables nonessential ligatures, unless overridden by the presence of kCTLigatureAttributeName.

Important

If you apply both kCTTrackingAttributeName and kCTKernAttributeName, kCTTrackingAttributeName supersedes kCTKernAttributeName.

## See Also

### Related Documentation

let kCTKernAttributeName: CFString

The amount to kern the next character.

let kCTLigatureAttributeName: CFString

The type of ligatures to use.

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

