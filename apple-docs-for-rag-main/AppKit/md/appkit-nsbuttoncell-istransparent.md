

- AppKit
- NSButtonCell
-  isTransparent 

Instance Property

# isTransparent

A Boolean value that indicates if the button is transparent.

macOS

``` source
@MainActor
var isTransparent: Bool { get set }
```

## Discussion

When the value of this property is true, the button is transparent, when it is false, the button is not transparent. The default value is false.

Setting this property redraws the button if necessary. A transparent button tracks the mouse and sends its action, but doesn’t draw. A transparent button is useful for sensitizing an area on the screen so that an action gets sent to a target when the area receives a mouse click.

## See Also

### Managing Graphics Attributes

var backgroundColor: NSColor?

The background color of the button.

var bezelStyle: NSButton.BezelStyle

The appearance of the button’s border, if it has one.

var gradientType: NSButton.GradientType

The gradient of the button’s border.

Deprecated

var imageDimsWhenDisabled: Bool

A Boolean value that indicates if the button’s image and text appear “dim” when the button is disabled.

var isOpaque: Bool

A Boolean value that indicates if the button is opaque.

var showsBorderOnlyWhileMouseInside: Bool

A Boolean value that indicates if the button displays its border only when the pointer is over it.

