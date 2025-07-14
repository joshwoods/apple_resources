

- Core Graphics
- CGColorSpace
-  itur_2020_PQ_EOTF Deprecated

Type Property

# itur_2020_PQ_EOTF

The recommendation of the International Telecommunication Union (ITU) Radiocommunication sector for the BT.2020 color space, with the PQ transfer function.

iOS 12.6–13.4DeprecatediPadOS 12.6–13.4DeprecatedMac Catalyst 13.1–13.4DeprecatedmacOS 10.14.6–10.15.4DeprecatedtvOS 12.0–13.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 5.0–6.2Deprecated

``` source
class let itur_2020_PQ_EOTF: CFString
```

Deprecated

No longer supported

## Discussion

This color space has the same colorimetry as itur_2020, but uses the Perceptual Quantizer (PQ) transfer function. A pixel value of `1.0` is assumed to be `100` nits. See the current active version of the BT.2100 recommendation on the ITU website (https://www.itu.int/).

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

