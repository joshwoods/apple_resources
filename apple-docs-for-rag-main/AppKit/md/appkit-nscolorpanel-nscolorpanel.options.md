

- AppKit
- NSColorPanel
-  NSColorPanel.Options 

Structure

# NSColorPanel.Options

The color modes that are enabled for a color panel.

macOS

``` source
struct Options
```

## Topics

### Color Panel Options

static var grayModeMask: NSColorPanel.Options

The grayscale-alpha color mode.

static var rgbModeMask: NSColorPanel.Options

The red-green-blue color mode.

static var cmykModeMask: NSColorPanel.Options

The cyan-magenta-yellow-black color mode.

static var hsbModeMask: NSColorPanel.Options

The hue-saturation-brightness color mode.

static var customPaletteModeMask: NSColorPanel.Options

The custom palette color mode.

static var colorListModeMask: NSColorPanel.Options

The custom color list mode.

static var wheelModeMask: NSColorPanel.Options

The color wheel mode.

static var crayonModeMask: NSColorPanel.Options

The crayon color mode.

static var allModesMask: NSColorPanel.Options

All color modes.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Setting Color Picker Modes

class func setPickerMode(NSColorPanel.Mode)

Specifies the color panel’s initial picker.

var mode: NSColorPanel.Mode

The mode of the receiver the mode is one of the modes allowed by the color mask.

enum Mode

A type defined for the `enum` constants specifying color panel modes.

class func setPickerMask(NSColorPanel.Options)

Determines which color selection modes are available in an application’s `NSColorPanel`.

