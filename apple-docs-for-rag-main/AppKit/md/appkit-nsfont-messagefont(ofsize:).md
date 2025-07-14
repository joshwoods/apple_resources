

- AppKit
- NSFont
-  messageFont(ofSize:) 

Type Method

# messageFont(ofSize:)

Returns the font used for standard interface items, such as button labels, menu items, and so on, in the specified size.

macOS

``` source
class func messageFont(ofSize fontSize: CGFloat) -> NSFont
```

## Parameters 

`fontSize`  

The size in points to which the font is scaled.

## Return Value

A font object of the specified size.

## Discussion

If `fontSize` is 0 or negative, returns this font at the default size. This method is equivalent to systemFont(ofSize:).

## See Also

### Related Documentation

init?(name: String, size: CGFloat)

Creates a font object for the specified font name and font size.

### Creating UI Element Fonts

class func labelFont(ofSize: CGFloat) -> NSFont

Returns the font used for standard interface labels in the specified size.

class func menuBarFont(ofSize: CGFloat) -> NSFont

Returns the font used for menu bar items, in the specified size.

class func menuFont(ofSize: CGFloat) -> NSFont

Returns the font used for menu items, in the specified size.

class func controlContentFont(ofSize: CGFloat) -> NSFont

Returns the font used for the content of controls in the specified size.

class func titleBarFont(ofSize: CGFloat) -> NSFont

Returns the font used for window title bars, in the specified size.

class func paletteFont(ofSize: CGFloat) -> NSFont

Returns the font used for palette window title bars, in the specified size.

class func toolTipsFont(ofSize: CGFloat) -> NSFont

Returns the font used for tool tips labels, in the specified size.

class var labelFontSize: CGFloat

Returns the size of the standard label font.

class func systemFontSize(for: NSControl.ControlSize) -> CGFloat

Returns the font size used for the specified control size.

