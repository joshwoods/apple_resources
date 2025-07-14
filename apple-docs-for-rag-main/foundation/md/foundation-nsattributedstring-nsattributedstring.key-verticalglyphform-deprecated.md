

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  verticalGlyphForm Deprecated

Type Property

# verticalGlyphForm

The vertical glyph form of the text.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–9.0Deprecated

``` source
static let verticalGlyphForm: NSAttributedString.Key
```

Deprecated

This attribute is not supported with TextKit 2

## Discussion

The value of this attribute is an NSNumber object containing an integer. The value `0` indicates horizontal text. The value `1` indicates vertical text. In iOS, horizontal text is always used and specifying a different value is undefined.

## See Also

### Deprecated Keys

static let expansion: NSAttributedString.Key

The expansion factor of the text.

Deprecated

static let obliqueness: NSAttributedString.Key

The obliqueness of the text.

Deprecated

static let characterShapeAttributeName: NSAttributedString.Key

The character shape attribute.

Deprecated

static let usesScreenFontsDocumentAttribute: NSAttributedString.Key

The screen fonts attribute.

Deprecated

