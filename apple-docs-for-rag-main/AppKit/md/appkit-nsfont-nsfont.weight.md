

- AppKit
- NSFont
-  NSFont.Weight 

Structure

# NSFont.Weight

System-defined font-weight values.

macOS

``` source
struct Weight
```

## Topics

### Font Weights

static let ultraLight: NSFont.Weight

The font weight for system ultra light font.

static let thin: NSFont.Weight

The font weight for system thin font.

static let light: NSFont.Weight

The font weight for system light font.

static let regular: NSFont.Weight

The font weight for system regular font.

static let medium: NSFont.Weight

The font weight for system medium font.

static let semibold: NSFont.Weight

The font weight for system semibold font.

static let bold: NSFont.Weight

The font weight for system bold font.

static let heavy: NSFont.Weight

The font weight for system heavy font.

static let black: NSFont.Weight

The font weight for system black font.

### Initializers

init(CGFloat)

init(rawValue: CGFloat)

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
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

struct TextStyle

Constants that specify the preferred text styles you use with fonts.

struct TextStyleOptionKey

The options that you apply when requesting the font or font descriptor of a preferred text style.

