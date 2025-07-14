

- AppKit
- NSFont
-  systemFontSize 

Type Property

# systemFontSize

Returns the size of the standard system font.

macOS

``` source
class var systemFontSize: CGFloat { get }
```

## Return Value

The standard system font size in points.

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

class var smallSystemFontSize: CGFloat

Returns the size of the standard small system font.

struct Weight

System-defined font-weight values.

struct TextStyle

Constants that specify the preferred text styles you use with fonts.

struct TextStyleOptionKey

The options that you apply when requesting the font or font descriptor of a preferred text style.

