

- AppKit
- NSBox
-  titlePosition 

Instance Property

# titlePosition

A constant representing the title position.

macOS

``` source
@MainActor
var titlePosition: NSBox.TitlePosition { get set }
```

## Discussion

A constant representing the position of the receiver’s title. See NSBox.TitlePosition for a list of these constants. If the new title position changes the size of the box’s border area, the content view is resized to absorb the difference, and the box is marked as needing redisplay.

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

var titleFont: NSFont

The font object used to draw the receiver’s title.

var titleCell: Any

The cell used to display the receiver’s title.

var titleRect: NSRect

The rectangle in which the receiver’s title is drawn.

