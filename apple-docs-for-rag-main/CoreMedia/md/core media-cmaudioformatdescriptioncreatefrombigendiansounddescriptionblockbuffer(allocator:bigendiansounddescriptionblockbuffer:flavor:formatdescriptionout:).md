

- Core Media
-  CMAudioFormatDescriptionCreateFromBigEndianSoundDescriptionBlockBuffer(allocator:bigEndianSoundDescriptionBlockBuffer:flavor:formatDescriptionOut:) 

Function

# CMAudioFormatDescriptionCreateFromBigEndianSoundDescriptionBlockBuffer(allocator:bigEndianSoundDescriptionBlockBuffer:flavor:formatDescriptionOut:)

Creates an audio format description from a big-endian sound description data structure in a buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMAudioFormatDescriptionCreateFromBigEndianSoundDescriptionBlockBuffer(
    allocator: CFAllocator?,
    bigEndianSoundDescriptionBlockBuffer soundDescriptionBlockBuffer: CMBlockBuffer,
    flavor: CMSoundDescriptionFlavor?,
    formatDescriptionOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

Allocator to use for allocating the CMAudioFormatDescription object. May be NULL.

`soundDescriptionBlockBuffer`  

CMBlockBuffer containing SoundDescription data structure in big-endian byte ordering.

`flavor`  

kCMSoundDescriptionFlavor constant or NULL for QuickTimeMovie flavor.

`formatDescriptionOut`  

Receives new CMAudioFormatDescription.

## See Also

### Working with Audio Descriptions

struct CMSoundDescriptionFlavor

Types that represent sound format descriptions.

func CMAudioFormatDescriptionCreateSummary(allocator: CFAllocator?, formatDescriptionArray: CFArray, flags: UInt32, formatDescriptionOut: UnsafeMutablePointer&lt;CMAudioFormatDescription?>) -> OSStatus

Creates a summary audio format description from an array of descriptions.

func CMAudioFormatDescriptionCreate(allocator: CFAllocator?, asbd: UnsafePointer&lt;AudioStreamBasicDescription>, layoutSize: Int, layout: UnsafePointer&lt;AudioChannelLayout>?, magicCookieSize: Int, magicCookie: UnsafeRawPointer?, extensions: CFDictionary?, formatDescriptionOut: UnsafeMutablePointer&lt;CMAudioFormatDescription?>) -> OSStatus

Creates a format description for an audio media stream.

func CMAudioFormatDescriptionEqual(CMAudioFormatDescription, otherFormatDescription: CMAudioFormatDescription, equalityMask: CMAudioFormatDescriptionMask, equalityMaskOut: UnsafeMutablePointer&lt;CMAudioFormatDescriptionMask>?) -> Bool

Returns a Boolean value that indicates whether the two audio format descriptions are equal.

func CMAudioFormatDescriptionGetChannelLayout(CMAudioFormatDescription, sizeOut: UnsafeMutablePointer&lt;Int>?) -> UnsafePointer&lt;AudioChannelLayout>?

Returns a read-only pointer to, and the size of, the audio channel layout inside an audio format description.

func CMAudioFormatDescriptionGetFormatList(CMAudioFormatDescription, sizeOut: UnsafeMutablePointer&lt;Int>?) -> UnsafePointer&lt;AudioFormatListItem>?

Returns a read-only pointer to, and size of, the array of audio format list item structures in an audio format description.

func CMAudioFormatDescriptionGetMagicCookie(CMAudioFormatDescription, sizeOut: UnsafeMutablePointer&lt;Int>?) -> UnsafeRawPointer?

Returns a read-only pointer to, and size of, the magic cookie in an audio format description.

func CMAudioFormatDescriptionGetMostCompatibleFormat(CMAudioFormatDescription) -> UnsafePointer&lt;AudioFormatListItem>?

Returns a read-only pointer to the appropriate audio format list item in an audio format description.

func CMAudioFormatDescriptionGetRichestDecodableFormat(CMAudioFormatDescription) -> UnsafePointer&lt;AudioFormatListItem>?

Returns a read-only pointer to the appropriate audio format list item in an audio format description.

func CMAudioFormatDescriptionGetStreamBasicDescription(CMAudioFormatDescription) -> UnsafePointer&lt;AudioStreamBasicDescription>?

Returns a read-only pointer to the audio stream description in an audio format description.

func CMDoesBigEndianSoundDescriptionRequireLegacyCBRSampleTableLayout(CMBlockBuffer, flavor: CMSoundDescriptionFlavor?) -> Bool

Returns a Boolean value that indicates whether the sample tables need to use the legacy constant bit-rate encoding layout.

func CMSwapBigEndianSoundDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a sound description data structure from big-endian to host-endian, in place.

func CMSwapHostEndianSoundDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a sound description data structure from host-endian to big-endian, in place.

func CMAudioFormatDescriptionCreateFromBigEndianSoundDescriptionData(allocator: CFAllocator?, bigEndianSoundDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMSoundDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMAudioFormatDescription?>) -> OSStatus

Creates an audio format description from a big-endian sound description data structure.

func CMAudioFormatDescriptionCopyAsBigEndianSoundDescriptionBlockBuffer(allocator: CFAllocator?, audioFormatDescription: CMAudioFormatDescription, flavor: CMSoundDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of an audio format description to a buffer in big-endian byte ordering.

