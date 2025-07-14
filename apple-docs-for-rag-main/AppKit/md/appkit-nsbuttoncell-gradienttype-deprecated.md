

- AppKit
- NSButtonCell
-  gradientType Deprecated

Instance Property

# gradientType

The gradient of the button’s border.

macOS 10.0–10.12Deprecated

``` source
@MainActor
var gradientType: NSButton.GradientType { get set }
```

Deprecated

The gradientType property is unused, and setting it has no effect.

## Discussion

The value of this property is a constant that specifies the gradient used for the button’s border. See NSButton.GradientType for a list of possible values.

If the button has no border, setting this property has no effect on the button’s appearance. A concave gradient is darkest in the top-left corner; a convex gradient is darkest in the bottom-right corner. Weak versus strong is how much contrast exists between the colors used in opposite corners.

Note

This property is currently unused by AppKit and has no effect.

## See Also

### Managing Graphics Attributes

var backgroundColor: NSColor?

The background color of the button.

var bezelStyle: NSButton.BezelStyle

The appearance of the button’s border, if it has one.

var imageDimsWhenDisabled: Bool

A Boolean value that indicates if the button’s image and text appear “dim” when the button is disabled.

var isOpaque: Bool

A Boolean value that indicates if the button is opaque.

var isTransparent: Bool

A Boolean value that indicates if the button is transparent.

var showsBorderOnlyWhileMouseInside: Bool

A Boolean value that indicates if the button displays its border only when the pointer is over it.

