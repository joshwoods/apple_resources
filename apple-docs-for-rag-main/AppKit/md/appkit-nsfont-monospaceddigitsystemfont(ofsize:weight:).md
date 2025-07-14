

- AppKit
- NSFont
-  monospacedDigitSystemFont(ofSize:weight:) 

Type Method

# monospacedDigitSystemFont(ofSize:weight:)

Returns a version of the standard system font that contains monospaced digit glyphs.

macOS 10.11+

``` source
class func monospacedDigitSystemFont(
    ofSize fontSize: CGFloat,
    weight: NSFont.Weight
) -> NSFont
```

## Parameters 

`fontSize`  

The desired font size specified in points. If you specify `0.0` or a negative number for this parameter, the method returns the system font at the default size.

`weight`  

The desired weight of font lines, specified as one of the constants in NSFont.Weight.

## Return Value

A font object containing the system font with monospace digits at the specified size and weight.

## Discussion

The font returned by this method has monospaced digit glyphs. Glyphs for other characters and symbols may be wider or narrower than the monospaced characters. To ensure the font uses fixed spacing for all characters, apply the fixedAdvance attribute to the any strings you render.

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

