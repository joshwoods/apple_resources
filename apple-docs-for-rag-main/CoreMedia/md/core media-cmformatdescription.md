

- Core Media
-  CMFormatDescription 

Class

# CMFormatDescription

An object that describes a media format descriptor.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
class CMFormatDescription
```

## Overview

A `CMFormatDescription` object is an object that describes media types (audio, video, muxed, and so on).

## Topics

### Inspecting Format Descriptions

var audioFormatList: [AudioFormatListItem]

The audio format list items that describe the audio formats.

var audioStreamBasicDescription: AudioStreamBasicDescription?

The audio stream description.

var audioChannelLayout: ManagedAudioChannelLayout?

The audio channel layout.

var dimensions: CMVideoDimensions

The encoded pixels not including the pixel aspect ratio or clean aperture tags.

var extensions: CMFormatDescription.Extensions

A dictionary that contains all of the extensions.

var frameDuration: CMTime

The duration of each frame.

var frameQuanta: UInt32

The frames per second for the time code, or the frame per tick for counter mode.

var identifiers: [String]

An array of metadata identifiers.

var magicCookie: Data?

A copy of the magic cookie, if any.

var mediaSubType: CMFormatDescription.MediaSubType

The media subtype.

var mediaType: CMFormatDescription.MediaType

The media type.

var mostCompatibleFormat: AudioFormatListItem?

The most compatible audio format list item.

var nalUnitHeaderLength: Int?

The size, in bytes, of the unit length field in an AVC or HEVC video sample or parameter set sample.

var parameterSets: CMFormatDescription.ParameterSetCollection

The parameter sets that an H.264 or HEVC format contains.

var richestDecodableFormat: AudioFormatListItem?

The audio format list item the system validates.

var timeCodeFlags: CMFormatDescription.TimeCode.Flag

The flags for the available time codes.

var tagCollections: [[CMTag]]?

The tag collections associated with this media.

func matchesTaggedBufferGroup([CMTaggedBuffer]) -> Bool

Whether the format description matches a set of tagged buffers.

### Working with Audio Descriptions

func withMagicCookie&lt;R>((UnsafeRawBufferPointer?) throws -> R) rethrows -> R

Returns the magic cookie.

### Working with Video Descriptions

func cleanAperture(originIsAtTopLeft: Bool) -> CGRect

Returns the clean aperture.

func matchesImageBuffer(CVImageBuffer) -> Bool

Returns a Boolean value that indicates whether the format description matches an image buffer.

func presentationDimensions(usePixelAspectRatio: Bool, useCleanAperture: Bool) -> CGSize

Returns the dimensions to take the pixel aspect ratio or clean aperture into account.

### Working with Metadata Descriptions

func keyWithLocalID(OSType) -> [String : CFPropertyList]?

Returns the metadata for the local identifier you specify.

### Working with Text Descriptions

func defaultStyle() throws -> (localFontID: Int, bold: Bool, italic: Bool, underline: Bool, fontSize: CGFloat, colorComponents: [CGFloat])

Returns the default text style.

func defaultTextBox(originIsAtTopLeft: Bool, heightOfTextTrack: CGFloat) throws -> CGRect

Returns the default text box.

func displayFlags() throws -> CMFormatDescription.Extensions.Value.TextDisplayFlags

Returns the display mode flags for the text media.

func fontName(localFontID: Int) throws -> String

Returns the font name for the local font identifier.

func justification() throws -> (horizontal: CMFormatDescription.Extensions.Value.TextJustification, vertical: CMFormatDescription.Extensions.Value.TextJustification)

Returns the horizontal and vertical justification.

### Comparing Format Descriptions

static func == (CMFormatDescription, CMFormatDescription) -> Bool

Equality is derived from

func equalTo(CMAudioFormatDescription, equalityMask: CMFormatDescription.EqualityMask) -> (Bool, equalityMask: CMFormatDescription.EqualityMask)

Evaluates equality for the parts of two audio format descriptions.

func equalTo(CMFormatDescription, extensionKeysToIgnore: [CMFormatDescription.Extensions.Key], sampleDescriptionExtensionAtomKeysToIgnore: [String]) -> Bool

Evaluates equality for the parts of two audio format descriptions, ignoring the extensions you specify.

### Errors

struct Error

A type that describes format description errors.

### Constants

static var extensionKeysCommonWithImageBuffers: [CMFormatDescription.Extensions.Key]

A constant that represents keys you use with video format description extensions and image buffers.

static var typeID: CFTypeID

A type identifier that corresponds to a description object.

struct MediaType

A type that describes format description media.

struct MediaSubType

A type that describes format description media subtypes.

struct TimeCode

A type that describes format description time codes.

struct EqualityMask

A type that describes format description equality masks.

struct Extensions

A type that describes format description extensions.

struct ParameterSetCollection

A type that describes format description parameter sets.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Format Description Types

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

