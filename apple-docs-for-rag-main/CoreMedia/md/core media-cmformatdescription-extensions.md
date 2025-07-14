

- Core Media
- CMFormatDescription
-  extensions 

Instance Property

# extensions

A dictionary that contains all of the extensions.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var extensions: CMFormatDescription.Extensions { get }
```

## See Also

### Inspecting Format Descriptions

var audioFormatList: [AudioFormatListItem]

The audio format list items that describe the audio formats.

var audioStreamBasicDescription: AudioStreamBasicDescription?

The audio stream description.

var audioChannelLayout: ManagedAudioChannelLayout?

The audio channel layout.

var dimensions: CMVideoDimensions

The encoded pixels not including the pixel aspect ratio or clean aperture tags.

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

