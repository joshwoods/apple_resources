

- AppKit
- NSFont
-  preferredFont(forTextStyle:options:) 

Type Method

# preferredFont(forTextStyle:options:)

Returns the font associated with the text style.

macOS 11.0+

``` source
class func preferredFont(
    forTextStyle style: NSFont.TextStyle,
    options: [NSFont.TextStyleOptionKey : Any] = [:]
) -> NSFont
```

## Parameters 

`style`  

The text style for which to return a font. See NSFont.TextStyle for available values.

`options`  

A dictionary you use to further configure the returned font. See NSFont.TextStyleOptionKey for a list of valid keys. Pass an empty dictionary to use the default configuration.

## Return Value

The font associated with the text style.

## See Also

### Creating System Fonts

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

struct TextStyle

Constants that specify the preferred text styles you use with fonts.

struct TextStyleOptionKey

The options that you apply when requesting the font or font descriptor of a preferred text style.

