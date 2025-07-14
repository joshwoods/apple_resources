

- AppKit
- NSColorPanel
-  NSColorPanel.Mode 

Enumeration

# NSColorPanel.Mode

A type defined for the `enum` constants specifying color panel modes.

macOS

``` source
enum Mode
```

## Topics

### Color Panel Modes

case none

No color panel mode.

case gray

The grayscale-alpha color mode.

case RGB

The red-green-blue color mode.

case CMYK

The cyan-magenta-yellow-black color mode.

case HSB

The hue-saturation-brightness color mode.

case customPalette

The custom palette color mode.

case colorList

The custom color list mode.

case wheel

The color wheel mode.

case crayon

The crayon picker mode.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting Color Picker Modes

class func setPickerMode(NSColorPanel.Mode)

Specifies the color panel’s initial picker.

var mode: NSColorPanel.Mode

The mode of the receiver the mode is one of the modes allowed by the color mask.

class func setPickerMask(NSColorPanel.Options)

Determines which color selection modes are available in an application’s `NSColorPanel`.

struct Options

The color modes that are enabled for a color panel.

