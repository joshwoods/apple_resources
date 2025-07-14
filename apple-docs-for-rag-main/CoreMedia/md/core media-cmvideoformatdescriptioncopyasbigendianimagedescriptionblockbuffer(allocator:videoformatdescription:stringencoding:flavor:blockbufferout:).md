

- Core Media
-  CMVideoFormatDescriptionCopyAsBigEndianImageDescriptionBlockBuffer(allocator:videoFormatDescription:stringEncoding:flavor:blockBufferOut:) 

Function

# CMVideoFormatDescriptionCopyAsBigEndianImageDescriptionBlockBuffer(allocator:videoFormatDescription:stringEncoding:flavor:blockBufferOut:)

Copies the contents of a video format description to a buffer in big-endian byte ordering.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMVideoFormatDescriptionCopyAsBigEndianImageDescriptionBlockBuffer(
    allocator: CFAllocator?,
    videoFormatDescription: CMVideoFormatDescription,
    stringEncoding: CFStringEncoding,
    flavor: CMImageDescriptionFlavor?,
    blockBufferOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator to use for allocating the `CMBlockBuffer` object. May be `NULL`.

`videoFormatDescription`  

The `CMVideoFormatDescription` to be copied.

`stringEncoding`  

Pass CFStringGetSystemEncoding() or `GetApplicationTextEncoding`.

`flavor`  

`kCMImageDescriptionFlavor` constant or `NULL` for QuickTimeMovie flavor.

`blockBufferOut`  

Receives a new `CMBlockBuffer` containing ImageDescription data structure in big-endian byte ordering.

## Discussion

On return, the caller owns the returned CMBlockBuffer, and must release it when done with it.

Note

The `dataRefIndex` field of the SampleDescription is intentionally filled with placeholder values (`0xFFFF`). The caller must overwrite these values with a valid `dataRefIndex` if writing the SampleDescription to a QuickTime/ISO file.

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

func CMVideoFormatDescriptionGetExtensionKeysCommonWithImageBuffers() -> CFArray

Returns an array of keys that you use for video format description extensions, image buffer attachments, and attributes.

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

func CMVideoFormatDescriptionCreateFromBigEndianImageDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianImageDescriptionBlockBuffer: CMBlockBuffer, stringEncoding: CFStringEncoding, flavor: CMImageDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMVideoFormatDescription?>) -> OSStatus

Creates a video format description from a big-endian image description inside a buffer.

func CMVideoFormatDescriptionCreateFromBigEndianImageDescriptionData(allocator: CFAllocator?, bigEndianImageDescriptionData: UnsafePointer&lt;UInt8>, size: Int, stringEncoding: CFStringEncoding, flavor: CMImageDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMVideoFormatDescription?>) -> OSStatus

Creates a video format description from a big-endian image description structure.

func CMSwapBigEndianImageDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts an image description data structure from big-endian to host-endian, in place.

func CMSwapHostEndianImageDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts an image description data structure from host-endian to big-endian, in place.

