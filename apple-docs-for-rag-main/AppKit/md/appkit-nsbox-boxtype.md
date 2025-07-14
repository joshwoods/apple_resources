

- AppKit
- NSBox
-  boxType 

Instance Property

# boxType

The receiver’s box type.

macOS

``` source
@MainActor
var boxType: NSBox.BoxType { get set }
```

## Discussion

A constant describing the type of box. These constants are described in NSBox.BoxType. By default, the box type of an `NSBox` is `NSBoxPrimary`.

## See Also

### Configuring Boxes

var borderRect: NSRect

The rectangle in which the receiver’s border is drawn.

var borderType: NSBorderType

The receiver’s border type.

Deprecated

var isTransparent: Bool

A Boolean value that indicates whether the receiver is transparent.

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

