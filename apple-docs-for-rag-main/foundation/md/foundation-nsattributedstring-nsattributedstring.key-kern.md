

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  kern 

Type Property

# kern

The kerning of the text.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let kern: NSAttributedString.Key
```

## Discussion

The value of this attribute is an NSNumber object containing a floating-point value. This value specifies the number of points by which to adjust kern-pair characters. Kerning prevents unwanted space from occurring between specific characters and depends on the font. The value `0` means kerning is disabled. The default value for this attribute is `0`.

## See Also

### Getting rendering attribute keys

static let backgroundColor: NSAttributedString.Key

The color of the background behind the text.

static let baselineOffset: NSAttributedString.Key

The vertical offset for the position of the text.

static let font: NSAttributedString.Key

The font of the text.

static let foregroundColor: NSAttributedString.Key

The color of the text.

static let glyphInfo: NSAttributedString.Key

The name of a glyph info object.

static let ligature: NSAttributedString.Key

The ligature of the text.

static let paragraphStyle: NSAttributedString.Key

The paragraph style of the text.

static let strikethroughColor: NSAttributedString.Key

The color of the strikethrough.

static let strikethroughStyle: NSAttributedString.Key

The strikethrough style of the text.

static let strokeColor: NSAttributedString.Key

The color of the stroke.

static let strokeWidth: NSAttributedString.Key

The width of the stroke.

static let superscript: NSAttributedString.Key

The superscript of the text.

static let tracking: NSAttributedString.Key

The amount to modify the default tracking.

static let underlineColor: NSAttributedString.Key

The color of the underline.

static let underlineStyle: NSAttributedString.Key

The underline style of the text.

