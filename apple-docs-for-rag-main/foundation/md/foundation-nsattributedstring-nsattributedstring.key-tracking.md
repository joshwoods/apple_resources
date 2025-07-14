

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  tracking 

Type Property

# tracking

The amount to modify the default tracking.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static let tracking: NSAttributedString.Key
```

## Discussion

The value of this attribute is an NSNumber object containing a floating-point value. The value represents the amount of space, in points, to add between the specified characters. A positive value increases the spacing between characters, and a negative value brings the characters closer together. Specify `0` to disable tracking.

The effect of this attribute is similar to the effect of kern, but the system treats tracking as trailing whitespace. A nonzero amount of tracking disables nonessential ligatures, unless the ligature attribute is present.

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

static let kern: NSAttributedString.Key

The kerning of the text.

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

static let underlineColor: NSAttributedString.Key

The color of the underline.

static let underlineStyle: NSAttributedString.Key

The underline style of the text.

