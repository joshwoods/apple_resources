

- AppKit
- NSColor
-  colorSpaceName Deprecated

Instance Property

# colorSpaceName

The name of the color space associated with the color.

macOS 10.0–10.14Deprecated

``` source
var colorSpaceName: NSColorSpaceName { get }
```

Deprecated

Use -type and NSColorType instead

## See Also

### Related Documentation

func usingColorSpaceName(NSColorSpaceName) -> NSColor?

Creates a new color object whose color is the same as the receiver’s, except that the new color object is in the specified color space.

Deprecated

func usingColorSpaceName(NSColorSpaceName?, device: [NSDeviceDescriptionKey : Any]?) -> NSColor?

Creates a new color object for the same color, but in the specified color space and specific to the provided device.

Deprecated

### Working with the Color Space

var type: NSColor.ColorType

The type of the color object.

func usingType(NSColor.ColorType) -> NSColor?

Returns a version of the color object that is compatible with the specified color type.

enum ColorType

Constants that indicate the color’s type, and which methods may be called on the color object.

var colorSpace: NSColorSpace

The color space associated with the color.

struct NSColorSpaceName

Constants that specify color space names.

