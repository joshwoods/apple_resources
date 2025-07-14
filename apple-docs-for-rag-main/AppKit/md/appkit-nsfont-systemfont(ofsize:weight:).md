

- AppKit
- NSFont
-  systemFont(ofSize:weight:) 

Type Method

# systemFont(ofSize:weight:)

Returns the standard system font with the specified size and weight.

macOS 10.11+

``` source
class func systemFont(
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

A font object containing the system font at the specified size and weight.

## Discussion

Use the returned font for standard interface items, including button labels, menu items, and so on that require a specific font style information.

## See Also

### Creating System Fonts

class func preferredFont(forTextStyle: NSFont.TextStyle, options: [NSFont.TextStyleOptionKey : Any]) -> NSFont

Returns the font associated with the text style.

class func systemFont(ofSize: CGFloat) -> NSFont

Returns the standard system font with the specified size.

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

