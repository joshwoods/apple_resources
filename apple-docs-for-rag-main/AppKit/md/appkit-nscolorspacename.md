

- AppKit
-  NSColorSpaceName 

Structure

# NSColorSpaceName

Constants that specify color space names.

macOS

``` source
struct NSColorSpaceName
```

## Topics

### Color Space Names

static let calibratedRGB: NSColorSpaceName

Calibrated color space with red, green, blue, and alpha components.

static let calibratedWhite: NSColorSpaceName

Calibrated color space with white and alpha components (pure white is 1.0)

static let custom: NSColorSpaceName

Custom `NSColorSpace` object and floating-point components describing a color in that space

static let deviceCMYK: NSColorSpaceName

Device-dependent color space with cyan, magenta, yellow, black, and alpha components

static let deviceRGB: NSColorSpaceName

Device-dependent color space with red, green, blue, and alpha components.

static let deviceWhite: NSColorSpaceName

Device-dependent color space with white and alpha components (pure white is 1.0)

static let named: NSColorSpaceName

Catalog name and color name components

static let pattern: NSColorSpaceName

Pattern image (tiled)

### Getting the Number of Components

var numberOfColorComponents: Int

Returns the number of color components in the specified color space.

### Initializers

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Working with the Color Space

var type: NSColor.ColorType

The type of the color object.

func usingType(NSColor.ColorType) -> NSColor?

Returns a version of the color object that is compatible with the specified color type.

enum ColorType

Constants that indicate the color’s type, and which methods may be called on the color object.

var colorSpace: NSColorSpace

The color space associated with the color.

var colorSpaceName: NSColorSpaceName

The name of the color space associated with the color.

Deprecated

