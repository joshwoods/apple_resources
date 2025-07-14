

- Accelerate
- Conversion
- Functions that perform any-to-any conversion
-  vImage Buffer Type Codes 

API Collection

# vImage Buffer Type Codes

Constants that specify the contents of vImage buffers.

## Topics

### Type

typealias vImageBufferTypeCode

Type codes, such as chrominance or luminance, for the contents of a vImage buffer.

### Constants

var kvImageBufferTypeCode_Alpha: Int

The buffer contains the alpha channel.

var kvImageBufferTypeCode_CGFormat: Int

The buffer contains data describable as a vImage Core Graphics image format as a single buffer.

var kvImageBufferTypeCode_CMYK_Black: Int

If the image has a CMYK color model, the buffer contains the black channel.

var kvImageBufferTypeCode_CMYK_Cyan: Int

If the image has a CMYK color model, the buffer contains the cyan channel.

var kvImageBufferTypeCode_CMYK_Magenta: Int

If the image has a CMYK color model, the buffer contains the magenta channel.

var kvImageBufferTypeCode_CMYK_Yellow: Int

If the image has a CMYK color model, the buffer contains the yellow channel.

var kvImageBufferTypeCode_CVPixelBuffer_YCbCr: Int

The buffer contains luminance and both chroma channels interleaved according to the vImageConstCVImageFormat image type.

var kvImageBufferTypeCode_Cb: Int

The buffer contains the blue chrominance channel.

var kvImageBufferTypeCode_Chroma: Int

The buffer contains both chrominance channels, interleaved.

var kvImageBufferTypeCode_Chunky: Int

The buffer contains chunky data not describable as a vImage Core Graphics image format.

var kvImageBufferTypeCode_ColorSpaceChannel1: Int

var kvImageBufferTypeCode_ColorSpaceChannel10: Int

var kvImageBufferTypeCode_ColorSpaceChannel11: Int

var kvImageBufferTypeCode_ColorSpaceChannel12: Int

var kvImageBufferTypeCode_ColorSpaceChannel13: Int

var kvImageBufferTypeCode_ColorSpaceChannel14: Int

var kvImageBufferTypeCode_ColorSpaceChannel15: Int

var kvImageBufferTypeCode_ColorSpaceChannel16: Int

var kvImageBufferTypeCode_ColorSpaceChannel2: Int

var kvImageBufferTypeCode_ColorSpaceChannel3: Int

var kvImageBufferTypeCode_ColorSpaceChannel4: Int

var kvImageBufferTypeCode_ColorSpaceChannel5: Int

var kvImageBufferTypeCode_ColorSpaceChannel6: Int

var kvImageBufferTypeCode_ColorSpaceChannel7: Int

var kvImageBufferTypeCode_ColorSpaceChannel8: Int

var kvImageBufferTypeCode_ColorSpaceChannel9: Int

var kvImageBufferTypeCode_Cr: Int

The buffer contains the red chrominance channel.

var kvImageBufferTypeCode_EndOfList: Int

End of list marker.

var kvImageBufferTypeCode_Indexed: Int

The buffer contains data in an indexed colorspace.

var kvImageBufferTypeCode_LAB_A: Int

If the image has a LAB color model, the buffer contains the *a\** channel.

var kvImageBufferTypeCode_LAB_B: Int

If the image has a LAB color model, the buffer contains the *b\** channel.

var kvImageBufferTypeCode_LAB_L: Int

If the image has a LAB color model, the buffer contains the *L\** channel.

var kvImageBufferTypeCode_Luminance: Int

The buffer contains only luminance data.

var kvImageBufferTypeCode_Monochrome: Int

The buffer contains a single color channel.

var kvImageBufferTypeCode_RGB_Blue: Int

If the image has a RGB color model, the buffer contains the blue channel.

var kvImageBufferTypeCode_RGB_Green: Int

If the image has a RGB color model, the buffer contains the green channel.

var kvImageBufferTypeCode_RGB_Red: Int

If the image has a RGB color model, the buffer contains the red channel.

var kvImageBufferTypeCode_UniqueFormatCount: Int

var kvImageBufferTypeCode_XYZ_X: Int

If the image has a XYZ color model, the buffer contains the *X* channel.

var kvImageBufferTypeCode_XYZ_Y: Int

If the image has a XYZ color model, the buffer contains the *Y* channel.

var kvImageBufferTypeCode_XYZ_Z: Int

If the image has a XYZ color model, the buffer contains the *Z* channel.

## See Also

### Performing a conversion

func vImageConvert_AnyToAny(vImageConverter, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Converts the pixels in a vImage buffer to another format, using the specified converter.

