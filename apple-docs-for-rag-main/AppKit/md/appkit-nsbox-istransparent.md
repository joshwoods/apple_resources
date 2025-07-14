

- AppKit
- NSBox
-  isTransparent 

Instance Property

# isTransparent

A Boolean value that indicates whether the receiver is transparent.

macOS 10.5+

``` source
@MainActor
var isTransparent: Bool { get set }
```

## Discussion

true when the receiver is transparent, false otherwise.

## See Also

### Configuring Boxes

var borderRect: NSRect

The rectangle in which the receiver’s border is drawn.

var boxType: NSBox.BoxType

The receiver’s box type.

var borderType: NSBorderType

The receiver’s border type.

Deprecated

var title: String

The receiver’s title.

var titleFont: NSFont

The font object used to draw the receiver’s title.

var titlePosition: NSBox.TitlePosition

A constant representing the title position.

var titleCell: Any

The cell used to display the receiver’s title.

var titleRect: NSRect

The rectangle in which the receiver’s title is drawn.

