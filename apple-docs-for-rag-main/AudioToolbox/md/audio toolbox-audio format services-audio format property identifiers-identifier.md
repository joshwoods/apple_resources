

- Audio Toolbox
- Audio Format Services
-  Audio Format Property Identifiers 

API Collection

# Audio Format Property Identifiers

Constants for use with the AudioFormatGetPropertyInfo(_:_:_:_:) and AudioFormatGetProperty(_:_:_:_:_:) functions.

## Topics

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

var kAudioFormatProperty_AvailableEncodeChannelLayoutTags: AudioFormatPropertyID

An array of `AudioChannelLayoutTag` values for the format and number of channels specified.

var kAudioFormatProperty_AvailableEncodeNumberChannels: AudioFormatPropertyID

An array of `UInt32` values indicating the number of channels that can be encoded.

var kAudioFormatProperty_ASBDFromMPEGPacket: AudioFormatPropertyID

An `AudioStreamBasicDescription` structure for a given MPEG Packet.

var kAudioFormatProperty_BitmapForLayoutTag: AudioFormatPropertyID

A bitmap for an `AudioChannelLayoutTag` value.

var kAudioFormatProperty_MatrixMixMap: AudioFormatPropertyID

A matrix of scaling coefficients for converting audio from one channel map to another in a standard way, if one is known. Otherwise, an error is returned. Set the `inSpecifier` parameter to an array of two pointers to `AudioChannelLayout` structures. The first points to the input layout, the second to the output layout. The value is a two dimensional array of `Float32` values, where the first dimension (rows) is the input channel and the second dimension (columns) is the output channel.

var kAudioFormatProperty_ChannelMap: AudioFormatPropertyID

An array of `SInt32` values for reordering input channels. Set the `inSpecifier` parameter to an array of two pointers to `AudioChannelLayout` structures. The first points to the input layout, the second to the output layout. The length of the output array is equal to the number of output channels.

var kAudioFormatProperty_NumberOfChannelsForLayout: AudioFormatPropertyID

The number of valid channels.

var kAudioFormatProperty_ValidateChannelLayout: AudioFormatPropertyID

The validity of an audio channel layout structure.

var kAudioFormatProperty_ChannelLayoutForTag: AudioFormatPropertyID

The channel descriptions for a standard channel layout.

var kAudioFormatProperty_TagForChannelLayout: AudioFormatPropertyID

An `AudioChannelLayoutTag` value for a layout.

var kAudioFormatProperty_ChannelLayoutName: AudioFormatPropertyID

The a name for a particular channel layout.

var kAudioFormatProperty_ChannelLayoutSimpleName: AudioFormatPropertyID

A simplified name for channel layout.

var kAudioFormatProperty_ChannelLayoutForBitmap: AudioFormatPropertyID

The channel descriptions for a standard channel layout,

var kAudioFormatProperty_ChannelName: AudioFormatPropertyID

The name for a particular channel.

var kAudioFormatProperty_ChannelShortName: AudioFormatPropertyID

An abbreviated name for a particular channel.

var kAudioFormatProperty_TagsForNumberOfChannels: AudioFormatPropertyID

An array of AudioChannelLayoutTag values for the number of channels specified. The specifier is a `UInt32` value that indicates the number of channels.

var kAudioFormatProperty_PanningMatrix: AudioFormatPropertyID

An array of `Float32` values, each representing the audio level of one channel.

var kAudioFormatProperty_BalanceFade: AudioFormatPropertyID

An array of coefficients, each a `Float32` value, for applying left/right audio balance and front/back audio fade.

var kAudioFormatProperty_ID3TagSize: AudioFormatPropertyID

A `UInt32` value indicating the ID3 tag size. The `inSpecifier` parameter must begin with the ID3 tag header and be at least 10 bytes in length.

var kAudioFormatProperty_ID3TagToDictionary: AudioFormatPropertyID

A `CFDictionary` object containing key/value pairs for the frames in the ID3 tag. Set the `inSpecifier` parameter to the entire ID3 tag. The caller must call the `CFRelease` function for the returned dictionary.

var kAudioFormatProperty_AreChannelLayoutsEquivalent: AudioFormatPropertyID

var kAudioFormatProperty_ChannelLayoutHash: AudioFormatPropertyID

var kAudioFormatProperty_FormatIsEncrypted: AudioFormatPropertyID

var kAudioFormatProperty_AvailableDecodeNumberChannels: AudioFormatPropertyID

var kAudioFormatProperty_FormatEmploysDependentPackets: AudioFormatPropertyID

## See Also

### Constants

enum AudioBalanceFadeType

Identifiers for audio balance fade types.

Audio Codec Component Constants

Audio codec component types.

Audio Codec Manufacturer and Implementation Types

Identifiers for audio codec manufacturers and implementation types.

enum AudioPanningMode

Identifiers for audio panning algorithms.

