

- AppKit
- NSBox
-  titleFont 

Instance Property

# titleFont

The font object used to draw the receiver’s title.

macOS

``` source
@MainActor
var titleFont: NSFont { get set }
```

## Discussion

By default, the title is drawn using the small system font (obtained using (smallSystemFontSize as the parameter of systemFont(ofSize:), both `NSFont` class methods). If the size of the new font is different from that of the old font, the content view is resized to absorb the difference.

## See Also

### Configuring Boxes

var borderRect: NSRect

The rectangle in which the receiver’s border is drawn.

var boxType: NSBox.BoxType

The receiver’s box type.

var borderType: NSBorderType

The receiver’s border type.

Deprecated

var isTransparent: Bool

A Boolean value that indicates whether the receiver is transparent.

var title: String

The receiver’s title.

var titlePosition: NSBox.TitlePosition

A constant representing the title position.

var titleCell: Any

The cell used to display the receiver’s title.

var titleRect: NSRect

The rectangle in which the receiver’s title is drawn.

