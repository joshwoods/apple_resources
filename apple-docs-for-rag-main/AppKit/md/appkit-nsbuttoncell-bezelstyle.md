

- AppKit
- NSButtonCell
-  bezelStyle 

Instance Property

# bezelStyle

The appearance of the button’s border, if it has one.

macOS

``` source
@MainActor
var bezelStyle: NSButton.BezelStyle { get set }
```

## Discussion

The value of this property is a constant that specifies the bezel style used by the button. See NSButton.BezelStyle for a list of possible values. If a button is borderless, the value of this property is ignored.

A button uses shading to look like it’s sticking out or pushed in. You can set the shading with the gradientType property.

## See Also

### Managing Graphics Attributes

var backgroundColor: NSColor?

The background color of the button.

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

