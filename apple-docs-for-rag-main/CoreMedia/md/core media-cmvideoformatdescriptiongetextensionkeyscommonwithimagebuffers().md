

- Core Media
-  CMVideoFormatDescriptionGetExtensionKeysCommonWithImageBuffers() 

Function

# CMVideoFormatDescriptionGetExtensionKeysCommonWithImageBuffers()

Returns an array of keys that you use for video format description extensions, image buffer attachments, and attributes.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMVideoFormatDescriptionGetExtensionKeysCommonWithImageBuffers() -> CFArray
```

## Discussion

When specifying a `CMFormatDescription` for a `CMSampleBuffer`, the format description must be consistent with formatting information attached to the `CVImageBuffer`. The width, height, and codecType must match (for `CVPixelBuffers` the codec type is given by `CVPixelBufferGetPixelFormatType`(pixelBuffer); for other `CVImageBuffers`, the codecType must be 0). The format description extensions must match the image buffer attachments for all the keys in the list returned by this function (if absent in either they must be absent in both). Currently, the list is:

- kCMFormatDescriptionExtension_CleanAperture

- kCMFormatDescriptionExtension_FieldCount

- kCMFormatDescriptionExtension_FieldDetail

- kCMFormatDescriptionExtension_PixelAspectRatio

- kCMFormatDescriptionExtension_ColorPrimaries

- kCMFormatDescriptionExtension_TransferFunction

- kCMFormatDescriptionExtension_GammaLevel

- kCMFormatDescriptionExtension_YCbCrMatrix

- kCMFormatDescriptionExtension_ICCProfile

- kCMFormatDescriptionExtension_ChromaLocationTopField

- kCMFormatDescriptionExtension_ChromaLocationBottomField

## See Also

### Working with Video Descriptions

struct CMImageDescriptionFlavor

Types that represent image format descriptions.

func CMVideoFormatDescriptionCreate(allocator: CFAllocator?, codecType: CMVideoCodecType, width: Int32, height: Int32, extensions: CFDictionary?, formatDescriptionOut: UnsafeMutablePointer&lt;CMVideoFormatDescription?>) -> OSStatus

Creates a format description for a video media stream.

func CMVideoFormatDescriptionCreateForImageBuffer(allocator: CFAllocator?, imageBuffer: CVImageBuffer, formatDescriptionOut: UnsafeMutablePointer&lt;CMVideoFormatDescription?>) -> OSStatus

Creates a format description for a video media stream by using an image buffer.

func CMVideoFormatDescriptionGetCleanAperture(CMVideoFormatDescription, originIsAtTopLeft: Bool) -> CGRect

Returns a rectangle that defines the portion of the encoded pixel dimensions that represent the image data that’s valid for displaying.

func CMVideoFormatDescriptionGetDimensions(CMVideoFormatDescription) -> CMVideoDimensions

Returns the video dimensions, in encoded pixels.

func CMVideoFormatDescriptionGetPresentationDimensions(CMVideoFormatDescription, usePixelAspectRatio: Bool, useCleanAperture: Bool) -> CGSize

Returns the dimensions after taking the pixel aspect ratio and clean aperture into account.

func CMVideoFormatDescriptionMatchesImageBuffer(CMVideoFormatDescription, imageBuffer: CVImageBuffer) -> Bool

Returns a Boolean value that indicates whether a format description matches an image buffer.

func CMVideoFormatDescriptionCreateFromH264ParameterSets(allocator: CFAllocator?, parameterSetCount: Int, parameterSetPointers: UnsafePointer&lt;UnsafePointer&lt;UInt8>>, parameterSetSizes: UnsafePointer&lt;Int>, nalUnitHeaderLength: Int32, formatDescriptionOut: UnsafeMutablePointer&lt;CMFormatDescription?>) -> OSStatus

Creates a format description for a video media stream that the parameter set describes.

func CMVideoFormatDescriptionCreateFromHEVCParameterSets(allocator: CFAllocator?, parameterSetCount: Int, parameterSetPointers: UnsafePointer&lt;UnsafePointer&lt;UInt8>>, parameterSetSizes: UnsafePointer&lt;Int>, nalUnitHeaderLength: Int32, extensions: CFDictionary?, formatDescriptionOut: UnsafeMutablePointer&lt;CMFormatDescription?>) -> OSStatus

Creates a format description for a video media stream using HEVC (H.265) parameter set NAL units.

func CMVideoFormatDescriptionGetH264ParameterSetAtIndex(CMFormatDescription, parameterSetIndex: Int, parameterSetPointerOut: UnsafeMutablePointer&lt;UnsafePointer&lt;UInt8>?>?, parameterSetSizeOut: UnsafeMutablePointer&lt;Int>?, parameterSetCountOut: UnsafeMutablePointer&lt;Int>?, nalUnitHeaderLengthOut: UnsafeMutablePointer&lt;Int32>?) -> OSStatus

Returns a parameter set that an H.264 format description contains.

func CMVideoFormatDescriptionCopyAsBigEndianImageDescriptionBlockBuffer(allocator: CFAllocator?, videoFormatDescription: CMVideoFormatDescription, stringEncoding: CFStringEncoding, flavor: CMImageDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a video format description to a buffer in big-endian byte ordering.

func CMVideoFormatDescriptionCreateFromBigEndianImageDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianImageDescriptionBlockBuffer: CMBlockBuffer, stringEncoding: CFStringEncoding, flavor: CMImageDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMVideoFormatDescription?>) -> OSStatus

Creates a video format description from a big-endian image description inside a buffer.

func CMVideoFormatDescriptionCreateFromBigEndianImageDescriptionData(allocator: CFAllocator?, bigEndianImageDescriptionData: UnsafePointer&lt;UInt8>, size: Int, stringEncoding: CFStringEncoding, flavor: CMImageDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMVideoFormatDescription?>) -> OSStatus

Creates a video format description from a big-endian image description structure.

func CMSwapBigEndianImageDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts an image description data structure from big-endian to host-endian, in place.

func CMSwapHostEndianImageDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts an image description data structure from host-endian to big-endian, in place.

