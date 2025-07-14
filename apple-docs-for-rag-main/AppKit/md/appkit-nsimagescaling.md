

- AppKit
-  NSImageScaling 

Enumeration

# NSImageScaling

Constants that specify a cell’s image scaling behavior.

macOS 10.5+

``` source
enum NSImageScaling
```

## Topics

### Constants

case scaleProportionallyDown

If it is too large for the destination, scale the image down while preserving the aspect ratio.

case scaleAxesIndependently

Scale each dimension to exactly fit destination.

case scaleNone

Do not scale the image.

case scaleProportionallyUpOrDown

Scale the image to its maximum possible dimensions while both staying within the destination area and preserving its aspect ratio.

### Type Properties

static var NSScaleNone: NSImageScalingDeprecated

static var NSScaleProportionally: NSImageScalingDeprecated

static var NSScaleToFit: NSImageScalingDeprecated

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum CellType

Constants for specifying how a cell represents its data (as text or as an image).

enum Attribute

Constants for specifying how a button behaves when pressed and how it displays its state.

enum ImagePosition

A constant for specifying the position of a button’s image relative to its title.

typealias StateValue

Constants for specifying a cell’s state and are used mostly for buttons.

Deprecated

struct StyleMask

Constants for specifying what happens when a button is pressed or is displaying its alternate state.

enum NSControlTint

Constants for specifying a cell’s tint color.

enum ControlSize

A constant for specifying a cell’s size.

struct HitResult

Constants used by the hitTest(for:in:of:) method to determine the effect of an event.

enum BackgroundStyle

Background styles to apply to a view’s cell.

Deprecated Scaling Constants

These are deprecated scaling constants.

Data Entry Types

These constants specify how a cell formats numeric data.

