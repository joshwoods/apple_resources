

- AppKit
- NSButtonCell
-  showsBorderOnlyWhileMouseInside 

Instance Property

# showsBorderOnlyWhileMouseInside

A Boolean value that indicates if the button displays its border only when the pointer is over it.

macOS

``` source
@MainActor
var showsBorderOnlyWhileMouseInside: Bool { get set }
```

## Discussion

When the value of this property is true if the button’s border is displayed only when the pointer is over the button and the button is active. When it is false, the border continues to display when the pointer is outside of the button’s bounds.

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

var isTransparent: Bool

A Boolean value that indicates if the button is transparent.

