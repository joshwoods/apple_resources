

- AppKit
- NSBox
-  title 

Instance Property

# title

The receiver’s title.

macOS

``` source
@MainActor
var title: String { get set }
```

## Discussion

The title of the `NSBox`. By default, a box’s title is “Title.” If the size of the new title is different from that of the old title, the content view is resized to absorb the difference.

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

var titleFont: NSFont

The font object used to draw the receiver’s title.

var titlePosition: NSBox.TitlePosition

A constant representing the title position.

var titleCell: Any

The cell used to display the receiver’s title.

var titleRect: NSRect

The rectangle in which the receiver’s title is drawn.

