

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  characterShapeAttributeName Deprecated

Type Property

# characterShapeAttributeName

The character shape attribute.

macOS 10.0–10.11Deprecated

``` source
static let characterShapeAttributeName: NSAttributedString.Key
```

Deprecated

This attribute is bound to a specific implementation of ATS feature and not generically supported by wide range of fonts. The majority of characters accessed through this API are now encoded in the Unicode standard. Use the CTFont feature API for fine control over character shape choices.

## Discussion

An integer value. The value is interpreted as Apple Type Services `kCharacterShapeType selector + 1`.

The character shape feature type (`kCharacterShapeType`) is used when a single font contains different appearances for the same character shape, and these shapes are not traditionally treated as swashes. It is needed for languages such as Chinese that have both traditional and simplified character sets.

The default value is 0 (disable). 1 is `kTraditionalCharactersSelector,` and so on. Refer to `` and Font Features in ATSUI Programming Guide for additional information.

## See Also

### Deprecated Keys

static let expansion: NSAttributedString.Key

The expansion factor of the text.

Deprecated

static let obliqueness: NSAttributedString.Key

The obliqueness of the text.

Deprecated

static let verticalGlyphForm: NSAttributedString.Key

The vertical glyph form of the text.

Deprecated

static let usesScreenFontsDocumentAttribute: NSAttributedString.Key

The screen fonts attribute.

Deprecated

