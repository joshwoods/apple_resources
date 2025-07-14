

- AppKit
- NSColor
-  colorSpace 

Instance Property

# colorSpace

The color space associated with the color.

macOS

``` source
var colorSpace: NSColorSpace { get }
```

## Discussion

Access this property only for colors that have an associated color space—specifically, colors not created by name or using a pattern image. Accessing it for other color types raises an exception. If you are unsure about a color object, convert it to an equivalent NSColorSpace-based object before calling this method.

It is safe to access this property for color objects created with the color space names calibratedWhite, NSCalibratedBlackColorSpace, calibratedRGB, deviceWhite, NSDeviceBlackColorSpace, deviceRGB, deviceCMYK, or custom—or with the NSColorSpace class methods corresponding to these names.

## See Also

### Related Documentation

func getComponents(UnsafeMutablePointer&lt;CGFloat>)

Returns the components of the color as an array.

var numberOfComponents: Int

The number of components in the color.

### Working with the Color Space

var type: NSColor.ColorType

The type of the color object.

func usingType(NSColor.ColorType) -> NSColor?

Returns a version of the color object that is compatible with the specified color type.

enum ColorType

Constants that indicate the color’s type, and which methods may be called on the color object.

var colorSpaceName: NSColorSpaceName

The name of the color space associated with the color.

Deprecated

struct NSColorSpaceName

Constants that specify color space names.

