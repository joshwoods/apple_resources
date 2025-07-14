

- AppKit
- NSButtonCell
-  imageDimsWhenDisabled 

Instance Property

# imageDimsWhenDisabled

A Boolean value that indicates if the button’s image and text appear “dim” when the button is disabled.

macOS

``` source
@MainActor
var imageDimsWhenDisabled: Bool { get set }
```

## Discussion

When the value of this property is true, the button’s image and text are dimmed when the button is disabled; when it is false, the image and text are not dimmed in the disabled state. By default, all button types except NSSwitchButton and NSRadioButton dim when disabled. When buttons of type NSSwitchButton and NSRadioButton are disabled, only the associated text dims.

The default setting for this state is reasserted whenever you invoke setButtonType(_:), so be sure to specify the button cell’s type before you set imageDimsWhenDisabled.

## See Also

### Related Documentation

func setButtonType(NSButton.ButtonType)

Sets how the button highlights while pressed and how it shows its state.

### Managing Graphics Attributes

var backgroundColor: NSColor?

The background color of the button.

var bezelStyle: NSButton.BezelStyle

The appearance of the button’s border, if it has one.

var gradientType: NSButton.GradientType

The gradient of the button’s border.

Deprecated

var isOpaque: Bool

A Boolean value that indicates if the button is opaque.

var isTransparent: Bool

A Boolean value that indicates if the button is transparent.

var showsBorderOnlyWhileMouseInside: Bool

A Boolean value that indicates if the button displays its border only when the pointer is over it.

