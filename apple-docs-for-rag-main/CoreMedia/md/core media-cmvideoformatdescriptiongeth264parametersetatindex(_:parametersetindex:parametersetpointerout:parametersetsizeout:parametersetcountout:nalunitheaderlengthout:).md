

- Core Media
-  CMVideoFormatDescriptionGetH264ParameterSetAtIndex(\_:parameterSetIndex:parameterSetPointerOut:parameterSetSizeOut:parameterSetCountOut:nalUnitHeaderLengthOut:) 

Function

# CMVideoFormatDescriptionGetH264ParameterSetAtIndex(\_:parameterSetIndex:parameterSetPointerOut:parameterSetSizeOut:parameterSetCountOut:nalUnitHeaderLengthOut:)

Returns a parameter set that an H.264 format description contains.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMVideoFormatDescriptionGetH264ParameterSetAtIndex(
    _ videoDesc: CMFormatDescription,
    parameterSetIndex: Int,
    parameterSetPointerOut: UnsafeMutablePointer?>?,
    parameterSetSizeOut: UnsafeMutablePointer?,
    parameterSetCountOut: UnsafeMutablePointer?,
    nalUnitHeaderLengthOut NALUnitHeaderLengthOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`videoDesc`  

The format description being interrogated.

`parameterSetIndex`  

Index of the parameter set to be returned in parameterSetPointerOut and parameterSetSizeOut. This parameter is ignored if both parameterSetPointerOut and parameterSetSizeOut are NULL.

`parameterSetPointerOut`  

Points to a pointer to receive the parameter set. Pass NULL if you do not want this information.

`parameterSetSizeOut`  

Points to a size_t to receive the size in bytes of the parameter set. Pass NULL if you do not want this information.

`parameterSetCountOut`  

Number of parameter sets in the AVC decoder configuration record contained in videoDesc. Pass NULL if you do not want this information.

`NALUnitHeaderLengthOut`  

Points to an int to receive the size, in bytes, of the NALUnitLength field in an AVC video sample or AVC parameter set sample. Pass NULL if you do not want this information.

## Discussion

This function parses the AVC decoder configuration record contained in a H.264 video format description and returns the parameter set NAL unit at the given index from it.Both parameterSetPointerOut and parameterSetSizeOut may be NULL, parameterSetCountOut will return the total number of parameter set NAL units contained in the AVC decoder configuration record.The parameter set NAL units returned will already have any emulation prevention bytes needed.The pointer returned in parameterSetPointerOut points to internal memory of videoDesc, and may only be accessed as long as a retain on videoDesc is held.

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

