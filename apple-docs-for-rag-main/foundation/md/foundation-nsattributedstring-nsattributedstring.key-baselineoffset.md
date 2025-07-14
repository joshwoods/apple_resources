

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  baselineOffset 

Type Property

# baselineOffset

The vertical offset for the position of the text.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let baselineOffset: NSAttributedString.Key
```

## Discussion

The value of this attribute is an NSNumber object containing a floating point value indicating the character’s offset from the baseline, in points. The default value is `0`.

Important

This attribute is different from kCTBaselineOffsetAttributeName; you need to use kCTBaselineOffsetAttributeName if you are writing code for Core Text.

## See Also

### Related Documentation

let kCTBaselineOffsetAttributeName: CFString

Vertical offset for text position.

### Getting rendering attribute keys

static let backgroundColor: NSAttributedString.Key

The color of the background behind the text.

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

static let tracking: NSAttributedString.Key

The amount to modify the default tracking.

static let underlineColor: NSAttributedString.Key

The color of the underline.

static let underlineStyle: NSAttributedString.Key

The underline style of the text.

