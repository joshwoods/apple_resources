

- Core Graphics
- CGColorSpace
-  genericRGBLinear 

Type Property

# genericRGBLinear

The generic RGB color space with a linear transfer function.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let genericRGBLinear: CFString
```

## Discussion

This color space has the same colorimetry as kCGColorSpaceGenericRGB, but with a linear transfer function.

## See Also

### Accessing System-Defined Color Spaces

class let displayP3: CFString

The Display P3 color space, created by Apple.

class let displayP3_HLG: CFString

The Display P3 color space, using the HLG transfer function.

class let displayP3_PQ_EOTF: CFString

The Display P3 color space, using the PQ transfer function.

Deprecated

class let extendedLinearDisplayP3: CFString

The Display P3 color space with a linear transfer function and extended-range values.

class let sRGB: CFString

The standard Red Green Blue (sRGB) color space.

class let linearSRGB: CFString

The sRGB color space with a linear transfer function.

class let extendedSRGB: CFString

The extended sRGB color space.

class let extendedLinearSRGB: CFString

The sRGB color space with a linear transfer function and extended-range values.

class let genericGrayGamma2_2: CFString

The generic gray color space that has an exponential transfer function with a power of 2.2.

class let extendedGray: CFString

The extended gray color space.

class let linearGray: CFString

The gray color space using a linear transfer function.

class let extendedLinearGray: CFString

The extended gray color space with a linear transfer function.

class let genericCMYK: CFString

The generic CMYK color space.

class let genericXYZ: CFString

The XYZ color space, as defined by the CIE 1931 standard.

class let genericLab: CFString

The generic LAB color space.

