

- Core Text
-  kCTLigatureAttributeName 

Global Variable

# kCTLigatureAttributeName

The type of ligatures to use.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCTLigatureAttributeName: CFString
```

## Discussion

The value associated with this attribute must be a CFNumber object. Default is an integer value of `1`. The ligature attribute determines what kinds of ligatures should be used when displaying the string. A value of `0` indicates that only ligatures essential for proper rendering of text should be used. A value of `1` indicates that standard ligatures should be used, and `2` indicates that all available ligatures should be used. Which ligatures are standard depends on the script and possibly the font. Arabic text, for example, requires ligatures for many character sequences but has a rich set of additional ligatures that combine characters. English text has no essential ligatures, and typically has only two standard ligatures, those for “fi” and “fl”—all others are considered more advanced or fancy.

## See Also

### Constants

let kCTCharacterShapeAttributeName: CFString

Controls glyph selection.

Deprecated

let kCTFontAttributeName: CFString

The font of the text to which this attribute applies.

let kCTKernAttributeName: CFString

The amount to kern the next character.

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

