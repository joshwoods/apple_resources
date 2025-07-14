

- AppKit
- NSColorPanel
-  mode 

Instance Property

# mode

The mode of the receiver the mode is one of the modes allowed by the color mask.

macOS

``` source
@MainActor
var mode: NSColorPanel.Mode { get set }
```

## See Also

### Setting Color Picker Modes

class func setPickerMode(NSColorPanel.Mode)

Specifies the color panel’s initial picker.

enum Mode

A type defined for the `enum` constants specifying color panel modes.

class func setPickerMask(NSColorPanel.Options)

Determines which color selection modes are available in an application’s `NSColorPanel`.

struct Options

The color modes that are enabled for a color panel.

