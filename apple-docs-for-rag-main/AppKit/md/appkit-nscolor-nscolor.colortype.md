

- AppKit
- NSColor
-  NSColor.ColorType 

Enumeration

# NSColor.ColorType

Constants that indicate the color’s type, and which methods may be called on the color object.

macOS

``` source
enum ColorType
```

## Topics

### Color Types

case componentBased

Colors that include floating-point color components and a color space.

case pattern

Colors that include an image to be used as a pattern.

case catalog

Colors that are retrieved from an asset catalog.

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

### Working with the Color Space

var type: NSColor.ColorType

The type of the color object.

func usingType(NSColor.ColorType) -> NSColor?

Returns a version of the color object that is compatible with the specified color type.

var colorSpace: NSColorSpace

The color space associated with the color.

var colorSpaceName: NSColorSpaceName

The name of the color space associated with the color.

Deprecated

struct NSColorSpaceName

Constants that specify color space names.

