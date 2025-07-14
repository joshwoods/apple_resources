

- Core Graphics
- CGColorSpace
-  itur_2020_HLG Deprecated

Type Property

# itur_2020_HLG

The recommendation of the International Telecommunication Union (ITU) Radiocommunication sector for the BT.2020 color space, with the HLG transfer function.

iOS 12.6–14.0DeprecatediPadOS 12.6–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.15.6–11.0DeprecatedtvOS 12.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 5.0–7.0Deprecated

``` source
class let itur_2020_HLG: CFString
```

Deprecated

No longer supported

## Discussion

This color space has the same colorimetry as itur_2020, but uses the Hybrid Log-Gamma (HLG) transfer function. Pixel values should be between `0.0` and `12.0`. See the current active version of the BT.2100 recommendation on the ITU website (https://www.itu.int/).

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

class let genericRGBLinear: CFString

The generic RGB color space with a linear transfer function.

class let genericXYZ: CFString

The XYZ color space, as defined by the CIE 1931 standard.

