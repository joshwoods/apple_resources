

- AppKit
- NSFont
-  systemFontSize(for:) 

Type Method

# systemFontSize(for:)

Returns the font size used for the specified control size.

macOS

``` source
class func systemFontSize(for controlSize: NSControl.ControlSize) -> CGFloat
```

## Parameters 

`controlSize`  

The control size constant.

## Return Value

The font size in points for the specified control size.

## Discussion

If `controlSize` does not correspond to a valid `NSControlSize`, returns the size of the standard system font.

## See Also

### Creating UI Element Fonts

class func labelFont(ofSize: CGFloat) -> NSFont

Returns the font used for standard interface labels in the specified size.

class func messageFont(ofSize: CGFloat) -> NSFont

Returns the font used for standard interface items, such as button labels, menu items, and so on, in the specified size.

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

