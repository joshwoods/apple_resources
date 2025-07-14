

- Core Video
- CVPixelFormatDescription
-  Pixel Format Identifiers 

API Collection

# Pixel Format Identifiers

Core Video does not provide support for all of these formats; this list defines only their names.

## Topics

### Constants

var kCVPixelFormatType_1Monochrome: OSType

1 bit indexed.

var kCVPixelFormatType_2Indexed: OSType

2-bit indexed.

var kCVPixelFormatType_4Indexed: OSType

4-bit indexed.

var kCVPixelFormatType_8Indexed: OSType

8-bit indexed.

var kCVPixelFormatType_1IndexedGray_WhiteIsZero: OSType

1 bit indexed gray, white is zero.

var kCVPixelFormatType_2IndexedGray_WhiteIsZero: OSType

2-bit indexed gray, white is zero.

var kCVPixelFormatType_4IndexedGray_WhiteIsZero: OSType

4-bit indexed gray, white is zero.

var kCVPixelFormatType_8IndexedGray_WhiteIsZero: OSType

8-bit indexed gray, white is zero.

var kCVPixelFormatType_16BE555: OSType

16-bit BE RGB 555.

var kCVPixelFormatType_16LE555: OSType

16-bit LE RGB 555.

var kCVPixelFormatType_16LE5551: OSType

16-bit LE RGB 5551.

var kCVPixelFormatType_16BE565: OSType

16-bit BE RGB 565.

var kCVPixelFormatType_16LE565: OSType

16-bit LE RGB 565.

var kCVPixelFormatType_24RGB: OSType

24-bit RGB.

var kCVPixelFormatType_24BGR: OSType

24-bit BGR.

var kCVPixelFormatType_32ARGB: OSType

32-bit ARGB.

var kCVPixelFormatType_32BGRA: OSType

32-bit BGRA.

var kCVPixelFormatType_32ABGR: OSType

32-bit ABGR.

var kCVPixelFormatType_32RGBA: OSType

32-bit RGBA.

var kCVPixelFormatType_64ARGB: OSType

64-bit ARGB, 16-bit big-endian samples.

var kCVPixelFormatType_48RGB: OSType

48-bit RGB, 16-bit big-endian samples.

var kCVPixelFormatType_32AlphaGray: OSType

32-bit AlphaGray, 16-bit big-endian samples, black is zero.

var kCVPixelFormatType_16Gray: OSType

16-bit Grayscale, 16-bit big-endian samples, black is zero.

var kCVPixelFormatType_30RGB: OSType

30-bit RGB, 10-bit big-endian samples, 2 unused padding bits (at least significant end).

var kCVPixelFormatType_422YpCbCr8: OSType

Component Y’CbCr 8-bit 4:2:2, ordered Cb Y’0 Cr Y’1.

var kCVPixelFormatType_4444YpCbCrA8: OSType

Component Y’CbCrA 8-bit 4:4:4:4, ordered Cb Y’ Cr A.

var kCVPixelFormatType_4444YpCbCrA8R: OSType

Component Y’CbCrA 8-bit 4:4:4:4, rendering format. Full range alpha, zero biased YUV, ordered A Y’ Cb Cr.

var kCVPixelFormatType_4444AYpCbCr8: OSType

Component Y’CbCrA 8-bit 4:4:4:4, ordered A Y’ Cb Cr, full range alpha, video range Y’CbCr.

var kCVPixelFormatType_4444AYpCbCr16: OSType

Component Y’CbCrA 16-bit 4:4:4:4, ordered A Y’ Cb Cr, full range alpha, video range Y’CbCr, 16-bit little-endian samples.

var kCVPixelFormatType_444YpCbCr8: OSType

Component Y’CbCr 8-bit 4:4:4.

var kCVPixelFormatType_422YpCbCr16: OSType

Component Y’CbCr 10,12,14,16-bit 4:2:2.

var kCVPixelFormatType_422YpCbCr10: OSType

Component Y’CbCr 10-bit 4:2:2.

var kCVPixelFormatType_444YpCbCr10: OSType

Component Y’CbCr 10-bit 4:4:4.

var kCVPixelFormatType_420YpCbCr8Planar: OSType

Planar Component Y’CbCr 8-bit 4:2:0. `baseAddr` points to a big-endian `CVPlanarPixelBufferInfo_YCbCrPlanar` struct.

var kCVPixelFormatType_420YpCbCr8PlanarFullRange: OSType

Planar Component Y’CbCr 8-bit 4:2:0, full range. `baseAddr` points to a big-endian `CVPlanarPixelBufferInfo_YCbCrPlanar` struct.

var kCVPixelFormatType_422YpCbCr_4A_8BiPlanar: OSType

First plane: Video-range Component Y’CbCr 8-bit 4:2:2, ordered Cb Y’0 Cr Y’1; second plane: alpha 8-bit 0-255.

var kCVPixelFormatType_420YpCbCr8BiPlanarVideoRange: OSType

Bi-Planar Component Y’CbCr 8-bit 4:2:0, video-range (luma=\[16,235\] chroma=\[16,240\]). `baseAddr` points to a big-endian `CVPlanarPixelBufferInfo_YCbCrBiPlanar` struct.

var kCVPixelFormatType_420YpCbCr8BiPlanarFullRange: OSType

Bi-Planar Component Y’CbCr 8-bit 4:2:0, full-range (luma=\[0,255\] chroma=\[1,255\]). `baseAddr` points to a big-endian `CVPlanarPixelBufferInfo_YCbCrBiPlanar` struct.

var kCVPixelFormatType_422YpCbCr8_yuvs: OSType

Component Y’CbCr 8-bit 4:2:2, ordered Y’0 Cb Y’1 Cr.

var kCVPixelFormatType_422YpCbCr8FullRange: OSType

Component Y’CbCr 8-bit 4:2:2, full range, ordered Y’0 Cb Y’1 Cr.

var kCVPixelFormatType_OneComponent8: OSType

8-bit one component, black is zero.

var kCVPixelFormatType_TwoComponent8: OSType

8-bit two component, black is zero.

var kCVPixelFormatType_OneComponent16Half: OSType

6-bit one component IEEE half-precision float, 16-bit little-endian samples.

var kCVPixelFormatType_OneComponent32Float: OSType

32-bit one component IEEE float, 32-bit little-endian samples.

var kCVPixelFormatType_TwoComponent16Half: OSType

16-bit two component IEEE half-precision float, 16-bit little-endian samples.

var kCVPixelFormatType_TwoComponent32Float: OSType

32-bit two component IEEE float, 32-bit little-endian samples.

var kCVPixelFormatType_64RGBAHalf: OSType

64-bit RGBA IEEE half-precision float, 16-bit little-endian samples.

var kCVPixelFormatType_128RGBAFloat: OSType

128-bit RGBA IEEE float, 32-bit little-endian samples.

var kCVPixelFormatType_14Bayer_BGGR: OSType

var kCVPixelFormatType_14Bayer_GBRG: OSType

var kCVPixelFormatType_14Bayer_GRBG: OSType

var kCVPixelFormatType_14Bayer_RGGB: OSType

var kCVPixelFormatType_30RGBLEPackedWideGamut: OSType

var kCVPixelFormatType_ARGB2101010LEPacked: OSType

var kCVPixelFormatType_420YpCbCr10BiPlanarFullRange: OSType

var kCVPixelFormatType_420YpCbCr10BiPlanarVideoRange: OSType

var kCVPixelFormatType_422YpCbCr10BiPlanarFullRange: OSType

var kCVPixelFormatType_422YpCbCr10BiPlanarVideoRange: OSType

var kCVPixelFormatType_444YpCbCr10BiPlanarFullRange: OSType

var kCVPixelFormatType_444YpCbCr10BiPlanarVideoRange: OSType

var kCVPixelFormatType_DepthFloat16: OSType

var kCVPixelFormatType_DepthFloat32: OSType

var kCVPixelFormatType_DisparityFloat16: OSType

var kCVPixelFormatType_DisparityFloat32: OSType

var kCVPixelFormatType_16VersatileBayer: OSType

var kCVPixelFormatType_40ARGBLEWideGamut: OSType

var kCVPixelFormatType_40ARGBLEWideGamutPremultiplied: OSType

var kCVPixelFormatType_420YpCbCr8VideoRange_8A_TriPlanar: OSType

var kCVPixelFormatType_422YpCbCr16BiPlanarVideoRange: OSType

var kCVPixelFormatType_422YpCbCr8BiPlanarFullRange: OSType

var kCVPixelFormatType_422YpCbCr8BiPlanarVideoRange: OSType

var kCVPixelFormatType_4444AYpCbCrFloat: OSType

var kCVPixelFormatType_444YpCbCr16BiPlanarVideoRange: OSType

var kCVPixelFormatType_444YpCbCr16VideoRange_16A_TriPlanar: OSType

var kCVPixelFormatType_444YpCbCr8BiPlanarFullRange: OSType

var kCVPixelFormatType_444YpCbCr8BiPlanarVideoRange: OSType

var kCVPixelFormatType_64RGBALE: OSType

var kCVPixelFormatType_64RGBA_DownscaledProResRAW: OSType

var kCVPixelFormatType_OneComponent10: OSType

var kCVPixelFormatType_OneComponent12: OSType

var kCVPixelFormatType_OneComponent16: OSType

var kCVPixelFormatType_TwoComponent16: OSType

## See Also

### Constants

Pixel Format Description Keys

The attributes of a pixel format.

