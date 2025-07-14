

- Accelerate
- Core Video interoperability
-  Core Video image format utilities 

API Collection

# Core Video image format utilities

Create, copy, and query Core Video image format descriptions.

## Topics

### Creating Core Video image formats

class vImageCVImageFormat

A mutable description of image encoding in a Core Video pixel buffer.

class vImageConstCVImageFormat

An immutable description of image encoding in a Core Video pixel buffer.

func vImageCVImageFormat_CreateWithCVPixelBuffer(CVPixelBuffer!) -> Unmanaged&lt;vImageCVImageFormat>!

Creates the description of the image encoding in an existing Core Video pixel buffer.

func vImageCVImageFormat_Create(UInt32, UnsafePointer&lt;vImage_ARGBToYpCbCrMatrix>!, CFString!, CGColorSpace!, Int32) -> Unmanaged&lt;vImageCVImageFormat>!

Creates the description of image encoding in a Core Video pixel buffer from the specified properties.

### Copying Core Video image formats

func vImageCVImageFormat_Copy(vImageConstCVImageFormat) -> Unmanaged&lt;vImageCVImageFormat>!

Returns a mutable copy of an immutable Core Video image format.

### Querying and setting the alpha hint

func vImageCVImageFormat_GetAlphaHint(vImageConstCVImageFormat) -> Int32

Returns the alpha hint of a Core Video image format.

func vImageCVImageFormat_SetAlphaHint(vImageCVImageFormat, Int32) -> vImage_Error

Sets the alpha hint of a Core Video image format.

### Querying and setting channel information

func vImageCVImageFormat_GetChannelCount(vImageConstCVImageFormat) -> UInt32

Returns the number of channels, including alpha, for the Core Video image format.

func vImageCVImageFormat_GetChannelDescription(vImageConstCVImageFormat, vImageBufferTypeCode) -> UnsafePointer&lt;vImageChannelDescription>!

Returns the channel description for a particular channel type.

func vImageCVImageFormat_CopyChannelDescription(vImageCVImageFormat, UnsafePointer&lt;vImageChannelDescription>, vImageBufferTypeCode) -> vImage_Error

Copies the channel description for a particular channel type to an image format.

func vImageCVImageFormat_GetChannelNames(vImageConstCVImageFormat) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns the names of the channels of a Core Video image format.

struct vImageChannelDescription

A description of the range and clamp limits for a pixel format.

### Querying and setting the chrominance siting

func vImageCVImageFormat_GetChromaSiting(vImageConstCVImageFormat) -> Unmanaged&lt;CFString>!

Returns the chrominance siting of a Core Video image format.

func vImageCVImageFormat_SetChromaSiting(vImageCVImageFormat, CFString!) -> vImage_Error

Sets the chrominance siting of a Core Video image format.

### Querying and setting the color space

func vImageCVImageFormat_GetColorSpace(vImageConstCVImageFormat) -> Unmanaged&lt;CGColorSpace>!

Returns the color space of a Core Video image format.

func vImageCVImageFormat_SetColorSpace(vImageCVImageFormat, CGColorSpace!) -> vImage_Error

Sets the color space of a Core Video image format.

### Querying and setting the conversion matrix

func vImageCVImageFormat_GetConversionMatrix(vImageConstCVImageFormat, UnsafeMutablePointer&lt;vImageMatrixType>!) -> UnsafeRawPointer!

Returns a pointer to the RGB-to-YpCbCr conversion matrix of a Core Video image format.

func vImageCVImageFormat_CopyConversionMatrix(vImageCVImageFormat, UnsafeRawPointer, vImageMatrixType) -> vImage_Error

Copies an RGB-to-YpCbCr conversion matrix to an image format’s internal matrix.

### Querying the image format code

func vImageCVImageFormat_GetFormatCode(vImageConstCVImageFormat) -> UInt32

Returns the four-character code that encodes the pixel format of a Core Video image format.

### Querying and setting the user data

func vImageCVImageFormat_GetUserData(vImageConstCVImageFormat) -> UnsafeMutableRawPointer!

Returns the user data of a Core Video image format.

func vImageCVImageFormat_SetUserData(vImageCVImageFormat, UnsafeMutableRawPointer!, ((vImageCVImageFormat?, UnsafeMutableRawPointer?) -> Void)!) -> vImage_Error

Sets the user data of a Core Video image format.

### Image format memory management

vImageCVImageFormat_Retain

Retains a Core Video image format.

vImageCVImageFormat_Release

Releases a Core Video image format.

