

- Application Services
- ColorSync Manager
-  Color Packing for Color Spaces 

# Color Packing for Color Spaces

Specify how color values are stored.

## Overview

The ColorSync bitmap data type CMBitmap includes a field that identifies the color space in which the color values of the bitmap image are expressed. This enumeration defines the types of packing for a color space’s storage format. The enumeration also defines an alpha channel that can be added as a component of a color value to define the degree of opacity or transparency of a color. These constants are combined with the constants described in Abstract Color Space Constants to create values that identify a bitmap’s color space. Your application does not specify color packing constants directly, but rather uses the combined constants, which are described in CMBitmapColorSpace.

### Version-Notes

The constants `cm48_16ColorPacking` and `cm64_16ColorPacking` were added in ColorSync version 2.5.

## Topics

### Constants

var cmNoColorPacking: Int

This constant is not used for ColorSync bitmaps.

var cmWord5ColorPacking: Int

The color values for three 5-bit color channels are stored consecutively in 16-bits, with the highest order bit unused.

var cmWord565ColorPacking: Int

var cmLong8ColorPacking: Int

var cmLong10ColorPacking: Int

The color values for three 10-bit color channels are stored consecutively in a 32-bit long, with the two highest order bits unused.

var cmAlphaFirstPacking: Int

An alpha channel is added to the color value as its first component.

var cmOneBitDirectPacking: Int

One bit is used as the pixel format. This storage format is used by the resulting bitmap pointed to by the `resultBitMap` field of the function CWMatchColors; the bitmap must be only 1 bit deep.

var cmAlphaLastPacking: Int

var cm8_8ColorPacking: Int

var cm16_8ColorPacking: Int

var cm24_8ColorPacking: Int

The color values for three 8-bit color channels are stored in consecutive bytes, for a total of 24 bits.

var cm32_8ColorPacking: Int

The color values for four 8-bit color channels are stored in consecutive bytes, for a total of 32 bits.

var cm40_8ColorPacking: Int

The color values for five 8-bit color channels are stored in consecutive bytes, for a total of 40 bits.

var cm48_8ColorPacking: Int

The color values for six 8-bit color channels are stored in consecutive bytes, for a total of 48 bits.

var cm56_8ColorPacking: Int

The color values for seven 8-bit color channels are stored in consecutive bytes, for a total of 56 bits.

var cm64_8ColorPacking: Int

The color values for eight 8-bit color channels are stored in consecutive bytes, for a total of 64 bits.

var cm32_16ColorPacking: Int

The color values for two 16-bit color channels are stored in a 32-bit word.

var cm48_16ColorPacking: Int

The color values for three 16-bit color channels are stored in 48 consecutive bits.

var cm64_16ColorPacking: Int

The color values for four 16-bit color channels are stored in 64 consecutive bits.

var cm32_32ColorPacking: Int

The color value for a 32-bit color channel is stored in a 32-bit word.

var cmLittleEndianPacking: Int

var cmReverseChannelPacking: Int

