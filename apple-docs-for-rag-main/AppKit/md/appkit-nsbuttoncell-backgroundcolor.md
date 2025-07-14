

- AppKit
- NSButtonCell
-  backgroundColor 

Instance Property

# backgroundColor

The background color of the button.

macOS

``` source
@NSCopying @MainActor
var backgroundColor: NSColor? { get set }
```

## Discussion

The background color is used only when drawing borderless buttons.

## See Also

### Managing Graphics Attributes

var bezelStyle: NSButton.BezelStyle

The appearance of the button’s border, if it has one.

var gradientType: NSButton.GradientType

The gradient of the button’s border.

Deprecated

var imageDimsWhenDisabled: Bool

A Boolean value that indicates if the button’s image and text appear “dim” when the button is disabled.

var isOpaque: Bool

A Boolean value that indicates if the button is opaque.

var isTransparent: Bool

A Boolean value that indicates if the button is transparent.

var showsBorderOnlyWhileMouseInside: Bool

A Boolean value that indicates if the button displays its border only when the pointer is over it.

