

- Audio Toolbox
-  kAudioFormatProperty_MatrixMixMap 

Global Variable

# kAudioFormatProperty_MatrixMixMap

A matrix of scaling coefficients for converting audio from one channel map to another in a standard way, if one is known. Otherwise, an error is returned. Set the `inSpecifier` parameter to an array of two pointers to `AudioChannelLayout` structures. The first points to the input layout, the second to the output layout. The value is a two dimensional array of `Float32` values, where the first dimension (rows) is the input channel and the second dimension (columns) is the output channel.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioFormatProperty_MatrixMixMap: AudioFormatPropertyID { get }
```

## See Also

### Constants

var kAudioFormatProperty_FormatInfo: AudioFormatPropertyID

General information about a format. Set the `inSpecifier` parameter to a magic cookie, or `NULL`. On input, the property value is an `AudioStreamBasicDescription` structure which should have at least the `mFormatID` field filled out. On output, the structure will be filled out as much as possible given the information known about the format and the contents of the magic cookie (if any is given). If multiple formats can be described by the `AudioStreamBasicDescription` and the associated magic cookie, this property will return the base level format.

var kAudioFormatProperty_FormatName: AudioFormatPropertyID

A name for a given format. Set the `inSpecifier` parameter to an `AudioStreamBasicDescription` structure describing the format to ask about. The value is a `CFStringRef` object. The caller is responsible for releasing the returned string. For some formats, such as linear PCM, you get back a descriptive string, for example, “16-bit, interleaved.”

var kAudioFormatProperty_EncodeFormatIDs: AudioFormatPropertyID

An array of `UInt32` values representing format identifiers for formats that are valid output formats for a converter. You must set the `inSpecifier` parameter to `NULL`.

var kAudioFormatProperty_DecodeFormatIDs: AudioFormatPropertyID

An array of `UInt32` values representing format identifiers for formats that are valid input formats for a converter. You must set the `inSpecifier` parameter to `NULL`.

var kAudioFormatProperty_FormatList: AudioFormatPropertyID

A list of structures describing the audio formats.

var kAudioFormatProperty_ASBDFromESDS: AudioFormatPropertyID

An `AudioStreamBasicDescription` structure for a given elementary stream descriptor (ESDS). Set the `inSpecifier` parameter to an ESDS. If multiple formats can be described by the ESDS, this property will return the base level format.

var kAudioFormatProperty_ChannelLayoutFromESDS: AudioFormatPropertyID

An `AudioChannelLayout` structure for a given elementary stream descriptor (ESDS).

var kAudioFormatProperty_OutputFormatList: AudioFormatPropertyID

A list of structures describing the audio formats.

var kAudioFormatProperty_FirstPlayableFormatFromList: AudioFormatPropertyID

The index of the first `AudioFormatListItem` that represents an audio format.

var kAudioFormatProperty_Encoders: AudioFormatPropertyID

An array of `AudioClassDescription` structures for all installed encoders for the specified audio format. Set the `inSpecifier` parameter to the format that you are interested in, for instance, `'aac'`.

var kAudioFormatProperty_Decoders: AudioFormatPropertyID

An array of `AudioClassDescription` structures for all installed decoders for the specified audio format. Set the `inSpecifier` parameter to the format that you are interested in, for instance, `'aac'`.

var kAudioFormatProperty_FormatIsVBR: AudioFormatPropertyID

Indicates whether or not a format has a variable number of bytes-per-packet.

var kAudioFormatProperty_FormatIsExternallyFramed: AudioFormatPropertyID

Indicates whether or not a format requires external framing information.

var kAudioFormatProperty_AvailableEncodeBitRates: AudioFormatPropertyID

An array of `AudioValueRange` structures describing all available bit rates.

var kAudioFormatProperty_AvailableEncodeSampleRates: AudioFormatPropertyID

An array of `AudioValueRange` structures.

