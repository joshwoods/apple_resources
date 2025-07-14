

- Audio Toolbox
-  kAudioFormatProperty_FormatList 

Global Variable

# kAudioFormatProperty_FormatList

A list of structures describing the audio formats.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioFormatProperty_FormatList: AudioFormatPropertyID { get }
```

## Discussion

A list of AudioFormatListItem structures describing the audio formats contained within the compressed bit stream, as described by the magic cookie. Set the `inSpecifier` parameter to an AudioFormatInfo structure.

## Discussion

The `mFormatID` field of the `AudioStreamBasicDescription` structure must filled in. Formats are returned in order from the most to least “rich,” with channel count taking the highest precedence, followed by sample rate.

The kAudioFormatProperty_FormatList property is the preferred method for discovering format information of the audio data. If the audio data can only be described by a single AudioFormatListItem, this property would be equivalent to using the kAudioFormatProperty_FormatInfo property, which should be used by the application as a fallback case, to ensure backward compatibility with existing systems when kAudioFormatProperty_FormatList is not present on the system.

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

var kAudioFormatProperty_AvailableEncodeChannelLayoutTags: AudioFormatPropertyID

An array of `AudioChannelLayoutTag` values for the format and number of channels specified.

