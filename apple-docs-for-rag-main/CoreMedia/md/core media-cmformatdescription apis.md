

- Core Media
-  CMFormatDescription APIs 

API Collection

# CMFormatDescription APIs

A media format descriptor that describes the samples in a sample buffer.

## Overview

`CMFormatDescriptions` are immutable Core Foundation objects that describe media data of various types, including audio, video, and muxed media data. There are two types of API: media-type-agnostic APIs (supported by all CMFormatDescriptions) and media-type-specific APIs. The media-type-agnostic APIs are prefixed with `CMFormatDescription`, and the media-type-specific APIs are prefixed with `CMAudioFormatDescription`, `CMVideoFormatDescription`, and so on.

## Topics

### Creating Format Descriptions

func CMFormatDescriptionCreate(allocator: CFAllocator?, mediaType: CMMediaType, mediaSubType: FourCharCode, extensions: CFDictionary?, formatDescriptionOut: UnsafeMutablePointer&lt;CMFormatDescription?>) -> OSStatus

Creates a format description for general use.

### Comparing Format Descriptions

func CMFormatDescriptionEqual(CMFormatDescription?, otherFormatDescription: CMFormatDescription?) -> Bool

Returns a Boolean value that indicates whether two format descriptions are equal.

func CMFormatDescriptionEqualIgnoringExtensionKeys(CMFormatDescription?, otherFormatDescription: CMFormatDescription?, extensionKeysToIgnore: CFTypeRef?, sampleDescriptionExtensionAtomKeysToIgnore: CFTypeRef?) -> Bool

Returns a Boolean value that indicates whether two format descriptions are equal, ignoring differences in the extension keys you specify.

### Inspecting Format Descriptions

func CMFormatDescriptionGetMediaType(CMFormatDescription) -> CMMediaType

Returns the media type of a format description.

func CMFormatDescriptionGetMediaSubType(CMFormatDescription) -> FourCharCode

Returns the media subtype of a format description.

func CMFormatDescriptionGetExtension(CMFormatDescription, extensionKey: CFString) -> CFPropertyList?

Returns an extension from the format description by using an extension key.

func CMFormatDescriptionGetExtensions(CMFormatDescription) -> CFDictionary?

Returns all of the extensions for a format description.

func CMFormatDescriptionGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier that identifies format description objects.

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

func CMAudioFormatDescriptionCreateFromBigEndianSoundDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianSoundDescriptionBlockBuffer: CMBlockBuffer, flavor: CMSoundDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMAudioFormatDescription?>) -> OSStatus

Creates an audio format description from a big-endian sound description data structure in a buffer.

func CMAudioFormatDescriptionCopyAsBigEndianSoundDescriptionBlockBuffer(allocator: CFAllocator?, audioFormatDescription: CMAudioFormatDescription, flavor: CMSoundDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of an audio format description to a buffer in big-endian byte ordering.

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

### Working with Muxed Descriptions

func CMMuxedFormatDescriptionCreate(allocator: CFAllocator?, muxType: CMMuxedStreamType, extensions: CFDictionary?, formatDescriptionOut: UnsafeMutablePointer&lt;CMMuxedFormatDescription?>) -> OSStatus

Creates a format description for a muxed media stream.

### Working with Metadata Descriptions

struct CMMetadataDescriptionFlavor

Types that represent metadata format descriptions.

func CMMetadataFormatDescriptionCreateWithKeys(allocator: CFAllocator?, metadataType: CMMetadataFormatType, keys: CFArray?, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description with the metadata keys you specify.

func CMMetadataFormatDescriptionGetKeyWithLocalID(CMMetadataFormatDescription, localKeyID: OSType) -> CFDictionary?

Returns the key for the local identifier.

func CMMetadataFormatDescriptionCopyAsBigEndianMetadataDescriptionBlockBuffer(allocator: CFAllocator?, metadataFormatDescription: CMMetadataFormatDescription, flavor: CMMetadataDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a metadata format description to a buffer in big-endian byte order.

func CMMetadataFormatDescriptionCreateByMergingMetadataFormatDescriptions(allocator: CFAllocator?, sourceDescription: CMMetadataFormatDescription, otherSourceDescription: CMMetadataFormatDescription, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description object by merging with another description.

func CMMetadataFormatDescriptionCreateFromBigEndianMetadataDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianMetadataDescriptionBlockBuffer: CMBlockBuffer, flavor: CMMetadataDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description from a big-endian metadata description structure inside a buffer.

func CMMetadataFormatDescriptionCreateFromBigEndianMetadataDescriptionData(allocator: CFAllocator?, bigEndianMetadataDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMMetadataDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description from a big-endian metadata description structure.

func CMMetadataFormatDescriptionCreateWithMetadataFormatDescriptionAndMetadataSpecifications(allocator: CFAllocator?, sourceDescription: CMMetadataFormatDescription, metadataSpecifications: CFArray, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description by extending an existing description with the values you specify.

func CMMetadataFormatDescriptionCreateWithMetadataSpecifications(allocator: CFAllocator?, metadataType: CMMetadataFormatType, metadataSpecifications: CFArray, formatDescriptionOut: UnsafeMutablePointer&lt;CMMetadataFormatDescription?>) -> OSStatus

Creates a metadata format description with the specifications you specify.

func CMSwapBigEndianMetadataDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a metadata description data structure from big-endian to host-endian, in place.

func CMSwapHostEndianMetadataDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a metadata description data structure from host-endian to big-endian, in place.

func CMMetadataFormatDescriptionGetIdentifiers(CMMetadataFormatDescription) -> CFArray?

Returns an array of metadata identifiers from a metadata format description.

### Working with Text Descriptions

struct CMTextDescriptionFlavor

Types that represent text format descriptions.

func CMTextFormatDescriptionGetDefaultStyle(CMFormatDescription, localFontIDOut: UnsafeMutablePointer&lt;UInt16>?, boldOut: UnsafeMutablePointer&lt;DarwinBoolean>?, italicOut: UnsafeMutablePointer&lt;DarwinBoolean>?, underlineOut: UnsafeMutablePointer&lt;DarwinBoolean>?, fontSizeOut: UnsafeMutablePointer&lt;CGFloat>?, colorComponentsOut: UnsafeMutablePointer&lt;CGFloat>?) -> OSStatus

Returns the default text style.

func CMTextFormatDescriptionGetDefaultTextBox(CMFormatDescription, originIsAtTopLeft: Bool, heightOfTextTrack: CGFloat, defaultTextBoxOut: UnsafeMutablePointer&lt;CGRect>) -> OSStatus

Returns the default text box.

func CMTextFormatDescriptionGetDisplayFlags(CMFormatDescription, displayFlagsOut: UnsafeMutablePointer&lt;CMTextDisplayFlags>) -> OSStatus

Returns the display flags.

func CMTextFormatDescriptionGetFontName(CMFormatDescription, localFontID: UInt16, fontNameOut: AutoreleasingUnsafeMutablePointer&lt;CFString?>) -> OSStatus

Returns a font name for a local font identifier.

func CMTextFormatDescriptionGetJustification(CMFormatDescription, horizontalOut: UnsafeMutablePointer&lt;CMTextJustificationValue>?, verticalOut: UnsafeMutablePointer&lt;CMTextJustificationValue>?) -> OSStatus

Returns the horizontal and vertical justification.

func CMTextFormatDescriptionCopyAsBigEndianTextDescriptionBlockBuffer(allocator: CFAllocator?, textFormatDescription: CMTextFormatDescription, flavor: CMTextDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a text format description to a buffer in big-endian byte order.

func CMTextFormatDescriptionCreateFromBigEndianTextDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianTextDescriptionBlockBuffer: CMBlockBuffer, flavor: CMTextDescriptionFlavor?, mediaType: CMMediaType, formatDescriptionOut: UnsafeMutablePointer&lt;CMTextFormatDescription?>) -> OSStatus

Creates a text format description from a big-endian text description structure inside a buffer.

func CMTextFormatDescriptionCreateFromBigEndianTextDescriptionData(allocator: CFAllocator?, bigEndianTextDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMTextDescriptionFlavor?, mediaType: CMMediaType, formatDescriptionOut: UnsafeMutablePointer&lt;CMTextFormatDescription?>) -> OSStatus

Creates a text format description from a big-endian text description structure.

func CMSwapBigEndianTextDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a text description structure from big-endian to host-endian, in place.

func CMSwapHostEndianTextDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a text description structure from host-endian to big-endian, in place.

### Working with Time Code Descriptions

struct CMTimeCodeDescriptionFlavor

Types that represent time code format descriptions.

func CMTimeCodeFormatDescriptionCreate(allocator: CFAllocator?, timeCodeFormatType: CMTimeCodeFormatType, frameDuration: CMTime, frameQuanta: UInt32, flags: UInt32, extensions: CFDictionary?, formatDescriptionOut: UnsafeMutablePointer&lt;CMTimeCodeFormatDescription?>) -> OSStatus

Creates a format description for time code media.

func CMTimeCodeFormatDescriptionGetFrameDuration(CMTimeCodeFormatDescription) -> CMTime

Returns the duration of each frame.

func CMTimeCodeFormatDescriptionGetFrameQuanta(CMTimeCodeFormatDescription) -> UInt32

Returns the frames per second for a time code, or frames per tick in counter mode.

func CMTimeCodeFormatDescriptionGetTimeCodeFlags(CMTimeCodeFormatDescription) -> UInt32

Returns time code flags.

func CMTimeCodeFormatDescriptionCopyAsBigEndianTimeCodeDescriptionBlockBuffer(allocator: CFAllocator?, timeCodeFormatDescription: CMTimeCodeFormatDescription, flavor: CMTimeCodeDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a time code format description to a buffer in big-endian byte order.

func CMTimeCodeFormatDescriptionCreateFromBigEndianTimeCodeDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianTimeCodeDescriptionBlockBuffer: CMBlockBuffer, flavor: CMTimeCodeDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMTimeCodeFormatDescription?>) -> OSStatus

Creates a time code format description from a big-endian time code description data structure in a buffer.

func CMTimeCodeFormatDescriptionCreateFromBigEndianTimeCodeDescriptionData(allocator: CFAllocator?, bigEndianTimeCodeDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMTimeCodeDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMTimeCodeFormatDescription?>) -> OSStatus

Creates a time code format description from a big-endian time code description structure.

func CMSwapBigEndianTimeCodeDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a time code description data structure from big-endian to host-endian, in place.

func CMSwapHostEndianTimeCodeDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a time code description data structure from host-endian to big-endian, in place.

### Working with Closed Captioning Descriptions

struct CMClosedCaptionDescriptionFlavor

Types that represent closed caption format descriptions.

func CMClosedCaptionFormatDescriptionCopyAsBigEndianClosedCaptionDescriptionBlockBuffer(allocator: CFAllocator?, closedCaptionFormatDescription: CMClosedCaptionFormatDescription, flavor: CMClosedCaptionDescriptionFlavor?, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>) -> OSStatus

Copies the contents of a closed caption format description to a buffer in big-endian byte order.

func CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionBlockBuffer(allocator: CFAllocator?, bigEndianClosedCaptionDescriptionBlockBuffer: CMBlockBuffer, flavor: CMClosedCaptionDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMClosedCaptionFormatDescription?>) -> OSStatus

Creates a closed caption format description from a big-endian closed caption description structure in a buffer.

func CMClosedCaptionFormatDescriptionCreateFromBigEndianClosedCaptionDescriptionData(allocator: CFAllocator?, bigEndianClosedCaptionDescriptionData: UnsafePointer&lt;UInt8>, size: Int, flavor: CMClosedCaptionDescriptionFlavor?, formatDescriptionOut: UnsafeMutablePointer&lt;CMClosedCaptionFormatDescription?>) -> OSStatus

Creates a closed caption format description from a big-endian closed caption description structure.

func CMSwapHostEndianClosedCaptionDescriptionToBig(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a closed caption description structure from host-endian to big-endian, in place.

func CMSwapBigEndianClosedCaptionDescriptionToHost(UnsafeMutablePointer&lt;UInt8>, Int) -> OSStatus

Converts a closed caption description structure from big-endian to host-endian, in place.

### Format Description Types

class CMFormatDescription

An object that describes a media format descriptor.

typealias CMAudioFormatDescription

A type you use to interact with audio format descriptions.

typealias CMClosedCaptionFormatDescription

A type you use to interact with closed caption format descriptions.

typealias CMMetadataFormatDescription

A type you use to interact with metadata format descriptions.

typealias CMMuxedFormatDescription

A type you use to interact with muxed format descriptions.

typealias CMTextFormatDescription

A type you use to interact with text format descriptions.

typealias CMTimeCodeFormatDescription

A type you use to interact with time code format descriptions.

typealias CMVideoFormatDescription

A type you use to interact with video format descriptions.

### Format Description Extension Keys

let kCMFormatDescriptionExtension_ContentColorVolume: CFString

let kCMFormatDescriptionExtension_HasAdditionalViews: CFString

let kCMFormatDescriptionExtension_HasLeftStereoEyeView: CFString

let kCMFormatDescriptionExtension_HasRightStereoEyeView: CFString

let kCMFormatDescriptionExtension_HeroEye: CFString

let kCMFormatDescriptionExtension_HorizontalDisparityAdjustment: CFString

let kCMFormatDescriptionExtension_LogTransferFunction: CFString

let kCMFormatDescriptionExtension_StereoCameraBaseline: CFString

let kCMFormatDescriptionHeroEye_Left: CFString

let kCMFormatDescriptionHeroEye_Right: CFString

### Format Types

typealias CMClosedCaptionFormatType

A closed caption format type.

typealias CMMetadataFormatType

A metadata format type.

Metadata Format Types

Constants that represent media format types.

typealias CMSubtitleFormatType

A type that represents a text subtitle format.

Subtitle Format Types

Constants that represent subtitle format types.

typealias CMTimeCodeFormatType

A time code format type.

Time Code Formats

Constants that represent time code format types.

typealias CMTextFormatType

A text format type.

typealias CMPixelFormatType

A pixel format type.

Tagged Buffer Group Format Types

### Data Types

struct CMVideoDimensions

A structure that represents video dimensions.

typealias CMAudioFormatDescriptionMask

A type for mask bits that represent parts of an audio format description.

typealias CMMediaType

Constants that represent media types.

typealias CMAudioCodecType

An audio codec type.

typealias CMVideoCodecType

A video codec type.

typealias CMTextDisplayFlags

An integer value that describes the display mode flags for text media.

typealias CMTextJustificationValue

An integer value that describes the justification modes for text media.

Media Type Constants

Constants that represent media types.

Muxed Stream Types

Constants that represent muxed stream types.

Audio Codec Types

Constants that represent audio codec types.

### Constants

Format Description Error Codes

Errors the system returns from format description calls.

Format Description Bridge Error Codes

Bridge errors the system returns from format description calls.

Format Description Constants

Constants that identify format descriptions.

Text Format Description Constants

Constants that identify text format descriptions.

Metadata Format Description Constants

Constants that identify metadata format descriptions.

Time Code Format Description Constants

Constants that identify time code format descriptions.

Pixel Aspect Ratio Extension Constants

Constants that identify pixel aspect ratio extensions.

Chroma Location Extension Constants

Constants that identify chroma location extensions.

Clean Aperture Extension Constants

Constants that identify clean aperture extensions.

Color Primary Extension Constants

Constants that identify color primary extensions.

Field Detail Extension Constants

Constants that identify field detail extensions.

Transfer Function Extension Constants

Constants that identify transfer function extensions.

MPEG-2-conformant Formats

Constants that identify MPEG-2 formats.

HEVC Temporal Level Info Constants

Constants that identify HEVC temporal level information.

YCbCrMatrix Extension Constants

Constants that identify YCbCrMatrix extensions.

Audio Format Description Mask Codes

Mask codes that identify audio formats.

Closed Caption Format Type Constants

Types that identify closed caption formats.

Time Code Flags

Flags that identify time codes.

Text Display Flags

Flags that identify text display methods.

Text Format Constants

Types that identify text formats.

Text Justification Constants

Types that identify text justifications.

Video Pixel Formats

Constants that identify video pixel formats.

Video Profile Constants

Constants that identify video profiles.

Video Codec Constants

Types that identify video codecs.

## See Also

### Sample Processing

CMSampleBuffer APIs

An object that contains zero or more media samples of a uniform media type.

CMBlockBuffer APIs

An object the system uses to move blocks of memory through a processing system.

struct CMTaggedBuffer

An instance of a media buffer containing metadata tags.

CMTaggedBufferGroup APIs

Objective-C types and interfaces for working with Core Media tagged buffer groups.

CMAttachment APIs

Add supporting metadata to sample buffers.

