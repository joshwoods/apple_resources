

- AppKit
- NSBox
-  borderType Deprecated

Instance Property

# borderType

The receiver’s border type.

macOS 10.0–10.15Deprecated

``` source
@MainActor
var borderType: NSBorderType { get set }
```

Deprecated

borderType is only applicable to NSBoxOldStyle, which is deprecated. To replace a borderType of NSNoBorder, use the \`transparent\` property.

## Discussion

A constant describing the type of border. Border types are defined in `NSView.h`. Currently, the following border types are defined: `NSNoBorder`,`NSLineBorder`,`NSBezelBorder`, `NSGrooveBorder`.

By default, the border type of an `NSBox` is `NSGrooveBorder`.

If the size of the new border is different from that of the old border, the content view is resized to absorb the difference, and the box is marked for redisplay.

## See Also

### Configuring Boxes

var borderRect: NSRect

The rectangle in which the receiver’s border is drawn.

var boxType: NSBox.BoxType

The receiver’s box type.

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

