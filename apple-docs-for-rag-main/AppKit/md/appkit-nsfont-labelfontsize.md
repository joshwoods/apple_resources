

- AppKit
- NSFont
-  labelFontSize 

Type Property

# labelFontSize

Returns the size of the standard label font.

macOS

``` source
class var labelFontSize: CGFloat { get }
```

## Return Value

The label font size in points.

## Discussion

The label font (Lucida Grande Regular 10 point) is used for the labels on toolbar buttons and to label tick marks on full-size sliders. See The macOS Environment in macOS Human Interface Guidelines for more information about system fonts.

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

class func systemFontSize(for: NSControl.ControlSize) -> CGFloat

Returns the font size used for the specified control size.

