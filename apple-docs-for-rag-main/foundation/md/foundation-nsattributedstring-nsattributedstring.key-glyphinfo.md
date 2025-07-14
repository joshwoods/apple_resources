

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  glyphInfo 

Type Property

# glyphInfo

The name of a glyph info object.

macOS 10.0+

``` source
static let glyphInfo: NSAttributedString.Key
```

## Discussion

The NSLayoutManager object assigns the glyph specified by this NSGlyphInfo object to the entire attribute range, provided that its contents match the specified base string, and that the specified glyph is available in the font specified by `NSFontAttributeName`.

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

