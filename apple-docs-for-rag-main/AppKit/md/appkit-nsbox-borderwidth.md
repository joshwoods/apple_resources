

- AppKit
- NSBox
-  borderWidth 

Instance Property

# borderWidth

The width of the receiver’s border when the receiver is a custom box with a simple line border.

macOS 10.5+

``` source
@MainActor
var borderWidth: CGFloat { get set }
```

## Discussion

The receiver’s border width. It must be a custom box—that is, it has a type of NSBox.BoxType.custom—and it must have a border style of NSBorderType.lineBorder.

### Special Considerations

Functional only when the receiver’s box type (boxType) is `NSBoxCustom` and its border type (borderType) is `NSLineBorder`.

## See Also

### Customizing

var borderColor: NSColor

The color of the receiver’s border when the receiver is a custom box with a simple line border.

var cornerRadius: CGFloat

The radius of the receiver’s corners when the receiver is a custom box with a simple line border.

var fillColor: NSColor

The color of the receiver’s background when the receiver is a custom box with a simple line border.

