

- AppKit
- NSFont
-  NSFont.TextStyle 

Structure

# NSFont.TextStyle

Constants that specify the preferred text styles you use with fonts.

macOS 11.0+

``` source
struct TextStyle
```

## Discussion

Pass these constants to preferredFont(forTextStyle:options:) or preferredFontDescriptor(forTextStyle:options:) to retrieve the corresponding font or font descriptor.

## Topics

### Constants

static let body: NSFont.TextStyle

The font you use for body text.

static let callout: NSFont.TextStyle

The font you use for callouts.

static let caption1: NSFont.TextStyle

The font you use for standard captions.

static let caption2: NSFont.TextStyle

The font you use for alternate captions.

static let footnote: NSFont.TextStyle

The font you use in footnotes.

static let headline: NSFont.TextStyle

The font you use for headings.

static let subheadline: NSFont.TextStyle

The font you use for subheadings.

static let largeTitle: NSFont.TextStyle

The font you use for large titles.

static let title1: NSFont.TextStyle

The font you use for first-level hierarchical headings.

static let title2: NSFont.TextStyle

The font you use for second-level hierarchical headings.

static let title3: NSFont.TextStyle

The font you use for third-level hierarchical headings.

### Initializers

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating System Fonts

class func preferredFont(forTextStyle: NSFont.TextStyle, options: [NSFont.TextStyleOptionKey : Any]) -> NSFont

Returns the font associated with the text style.

class func systemFont(ofSize: CGFloat) -> NSFont

Returns the standard system font with the specified size.

class func systemFont(ofSize: CGFloat, weight: NSFont.Weight) -> NSFont

Returns the standard system font with the specified size and weight.

class func boldSystemFont(ofSize: CGFloat) -> NSFont

Returns the standard system font in boldface type with the specified size.

class func monospacedSystemFont(ofSize: CGFloat, weight: NSFont.Weight) -> NSFont

Returns a monospace version of the system font with the specified size and weight.

class func monospacedDigitSystemFont(ofSize: CGFloat, weight: NSFont.Weight) -> NSFont

Returns a version of the standard system font that contains monospaced digit glyphs.

class var systemFontSize: CGFloat

Returns the size of the standard system font.

class var smallSystemFontSize: CGFloat

Returns the size of the standard small system font.

struct Weight

System-defined font-weight values.

struct TextStyleOptionKey

The options that you apply when requesting the font or font descriptor of a preferred text style.

