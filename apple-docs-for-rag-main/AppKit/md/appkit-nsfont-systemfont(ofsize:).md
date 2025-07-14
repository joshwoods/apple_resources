

- AppKit
- NSFont
-  systemFont(ofSize:) 

Type Method

# systemFont(ofSize:)

Returns the standard system font with the specified size.

macOS

``` source
class func systemFont(ofSize fontSize: CGFloat) -> NSFont
```

## Parameters 

`fontSize`  

The desired font size specified in points. If you specify `0.0` or a negative number for this parameter, the method returns the system font at the default size.

## Return Value

A font object containing the system font at the specified size.

## Discussion

Use the returned font for standard interface items, including button labels, menu items, and so on that use the default font appearance.

## See Also

### Related Documentation

init?(name: String, size: CGFloat)

Creates a font object for the specified font name and font size.

class func userFixedPitchFont(ofSize: CGFloat) -> NSFont?

Returns the font used by default for documents and other text under the user’s control (that is, text whose font the user can normally change), when that font should be fixed-pitch, in the specified size.

class func userFont(ofSize: CGFloat) -> NSFont?

Returns the font used by default for documents and other text under the user’s control (that is, text whose font the user can normally change), in the specified size.

### Creating System Fonts

class func preferredFont(forTextStyle: NSFont.TextStyle, options: [NSFont.TextStyleOptionKey : Any]) -> NSFont

Returns the font associated with the text style.

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

