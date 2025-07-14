

- Core Graphics
- CGColorSpace
-  displayP3 

Type Property

# displayP3

The Display P3 color space, created by Apple.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.2+tvOS 9.2+visionOS 1.0+watchOS 2.2+

``` source
class let displayP3: CFString
```

## Discussion

This color space uses the DCI P3 primaries, a D65 white point, and the sRGB transfer function.

## See Also

### Accessing System-Defined Color Spaces

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

class let genericRGBLinear: CFString

The generic RGB color space with a linear transfer function.

class let genericXYZ: CFString

The XYZ color space, as defined by the CIE 1931 standard.

class let genericLab: CFString

The generic LAB color space.

