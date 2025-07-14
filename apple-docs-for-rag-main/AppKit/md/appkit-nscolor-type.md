

- AppKit
- NSColor
-  type 

Instance Property

# type

The type of the color object.

macOS 10.13+

``` source
var type: NSColor.ColorType { get }
```

## Discussion

A color object’s type determines which of its methods and properties you may access. For example, if the type is NSColor.ColorType.pattern, you may safely access the patternImage property.

## See Also

### Working with the Color Space

func usingType(NSColor.ColorType) -> NSColor?

Returns a version of the color object that is compatible with the specified color type.

enum ColorType

Constants that indicate the color’s type, and which methods may be called on the color object.

var colorSpace: NSColorSpace

The color space associated with the color.

var colorSpaceName: NSColorSpaceName

The name of the color space associated with the color.

Deprecated

struct NSColorSpaceName

Constants that specify color space names.

