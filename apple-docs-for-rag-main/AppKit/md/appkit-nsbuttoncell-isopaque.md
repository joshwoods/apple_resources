

- AppKit
- NSButtonCell
-  isOpaque 

Instance Property

# isOpaque

A Boolean value that indicates if the button is opaque.

macOS

``` source
@MainActor
var isOpaque: Bool { get }
```

## Discussion

When the value of this property is true, the button draws over every pixel in its frame. Note that a button cell is opaque only if it isn’t transparent and if it has a border. The default value of this property is true.

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

var isTransparent: Bool

A Boolean value that indicates if the button is transparent.

var showsBorderOnlyWhileMouseInside: Bool

A Boolean value that indicates if the button displays its border only when the pointer is over it.

