

- Accelerate
- Conversion
-  Functions that perform any-to-any conversion 

API Collection

# Functions that perform any-to-any conversion

Convert between Core Video or Core Graphics image data of arbitrary color spaces and bit depths.

## Topics

### Creating a converter

class vImageConverter

A description of a conversion from one image format to another.

func vImageConverter_CreateWithCGImageFormat(UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts from one vImage Core Graphics image format to another.

func vImageConverter_CreateWithCGColorConversionInfo(CGColorConversionInfo, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates an any-to-any converter that uses a color conversion information object to convert from one image format to another.

func vImageConverter_CreateForCGToCVImageFormat(UnsafePointer&lt;vImage_CGImageFormat>, vImageCVImageFormat, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts a Core Graphics-formatted image to a Core Video-formatted image.

func vImageConverter_CreateForCVToCGImageFormat(vImageCVImageFormat, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts a Core Video-formatted image to a Core Graphics-formatted image.

func vImageConverter_CreateWithColorSyncCodeFragment(CFTypeRef, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>!, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter to convert from one vImage Core Graphics image format to another, using custom ColorSync transform.

### Performing a conversion

func vImageConvert_AnyToAny(vImageConverter, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Converts the pixels in a vImage buffer to another format, using the specified converter.

vImage Buffer Type Codes

Constants that specify the contents of vImage buffers.

### Querying a converter’s properties

func vImageConverter_MustOperateOutOfPlace(vImageConverter, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, vImage_Flags) -> vImage_Error

Determines whether a converter is capable of operating in place.

func vImageConverter_GetSourceBufferOrder(vImageConverter) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns a list of vImage source buffer channel names, specifying the order of planes.

func vImageConverter_GetDestinationBufferOrder(vImageConverter) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns a list of vImage destination buffer channel names, specifying the order of planes.

func vImageConverter_GetNumberOfSourceBuffers(vImageConverter) -> UInt

Returns the number of source buffers consumed by the converter.

func vImageConverter_GetNumberOfDestinationBuffers(vImageConverter) -> UInt

Returns the number of destination buffers written to by the converter.

### Memory management

vImageConverter_Retain

Retains a vImage converter.

vImageConverter_Release

Releases a vImage converter.

## See Also

### Converting any-to-any

Building a basic image conversion workflow

Learn the fundamentals of the convert-any-to-any function by converting a CMYK image to an RGB image.

Converting chroma-subsampled images

Create vImage buffers with the correct dimensions to convert to and from images with subsampled chroma information.

