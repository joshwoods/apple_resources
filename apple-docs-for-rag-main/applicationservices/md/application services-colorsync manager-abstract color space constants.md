

- Application Services
- ColorSync Manager
-  Abstract Color Space Constants 

# Abstract Color Space Constants

Specify values that represent general color spaces.

## Overview

The data type CMBitmap defines a bitmap for an image whose colors can be matched with the function CWMatchColors or color-checked with the function CWCheckColors.

The `space` field of the `CMBitmap` type definition identifies the color space in which the colors of the bitmap image are specified. A color space is characterized by a number of components or dimensions, with each component carrying a numeric value. These values together make up the color value. A color space also specifies the format in which the color value is stored. For bitmaps in which color values are packed, the `space` field of the `CMBitmap` data type holds a constant that defines the color space and the packing format.

For the `CWMatchBitmap` function to perform color matching successfully, the color space specified in the `CMBitmap` data type’s `space` field must correspond to the color space specified in the profile’s `dataColorSpace` field. The source bitmap and source profile values must match and the destination bitmap and destination profile values must match. For the `CWCheckBitMap` function to perform color checking successfully, the source profile’s `dataColorSpace` field value and the `space` field value of the source bitmap must specify the same color space. These functions will execute successfully as long as the color spaces are the same without regard for the packing format specified by the bitmap.

This enumeration defines constants for abstract color spaces which, when combined with a packing format constant as described in Color Packing for Color Spaces, can be used in the `space` field of the `CMBitmap` structure. The combined constants are shown in CMBitmapColorSpace.

### Version-Notes

The constants `cmRGBASpace` and `cmGrayASpace` were moved to this enum from CMBitmapColorSpace in ColorSync version 2.5.

## Topics

### Constants

var cmNoSpace: Int

The ColorSync Manager does not use this constant.

var cmRGBSpace: Int

An RGB color space composed of red, green, and blue components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

var cmCMYKSpace: Int

A CMYK color space composed of cyan, magenta, yellow, and black. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

var cmHSVSpace: Int

An HSV color space composed of hue, saturation, and value components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

var cmHLSSpace: Int

An HLS color space composed of hue, lightness, and saturation components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

var cmYXYSpace: Int

A Yxy color space composed of Y, x, and y components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

var cmXYZSpace: Int

An XYZ color space composed of X, Y, and Z components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

var cmLUVSpace: Int

An L\*u\*v\* color space composed of L\*, u\*, and v\* components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

var cmLABSpace: Int

An L\*a\*b\* color space composed of L\*, a\*, b\* components. A bitmap never uses this constant alone. Instead, this color space is always combined with a packing format describing the amount of storage per component.

var cmReservedSpace1: Int

This field is reserved for use by QuickDraw GX.

var cmGraySpace: Int

A luminance color space with a single component, gray.

var cmReservedSpace2: Int

This field is reserved for use by QuickDraw GX.

var cmGamutResultSpace: Int

var cmNamedIndexedSpace: Int

A named indexed color space.

var cmMCFiveSpace: Int

A five-channel multichannel (HiFi) data color space.

var cmMCSixSpace: Int

A six-channel multichannel (HiFi) data color space.

var cmMCSevenSpace: Int

A seven-channel multichannel (HiFi) data color space.

var cmMCEightSpace: Int

An eight-channel multichannel (HiFi) data color space.

var cmAlphaPmulSpace: Int

A premultiplied alpha channel component is added to the color value.

var cmAlphaSpace: Int

An alpha channel component is added to the color value.

var cmRGBASpace: Int

var cmGrayASpace: Int

A luminance color space with two components, a gray component followed by an alpha channel component. Each component value is 16 bits.

var cmRGBAPmulSpace: Int

var cmGrayAPmulSpace: Int

