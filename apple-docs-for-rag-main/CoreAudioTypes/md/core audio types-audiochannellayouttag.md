

- Core Audio Types
-  AudioChannelLayoutTag 

Type Alias

# AudioChannelLayoutTag

Identifies a previously-defined channel layout.

iOS 2.0+iPadOS 2.0+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
typealias AudioChannelLayoutTag = UInt32
```

## Discussion

This data type is used for the `mChannelLayoutTag` field of the AudioChannelLayout structure. See Audio Channel Layout Tags for possible values.

## See Also

### Accessing the Data

var mChannelBitmap: AudioChannelBitmap

If `mChannelLayoutTag` is set to `kAudioChannelLayoutTag_UseChannelBitmap`, this field is the channel-use bitmap.

struct AudioChannelBitmap

The supported channel bitmaps to use when defining channel layouts.

var mChannelDescriptions: AudioChannelDescription

A variable length array of `mNumberChannelDescription` elements that describes a layout. If the `mChannelLayoutTag` field is set to `kAudioChannelLayoutTag_UseChannelDescriptions`, use this field to describe the layout.

var mChannelLayoutTag: AudioChannelLayoutTag

The `AudioChannelLayoutTag` value that indicates the layout. See Audio Channel Layout Tags for possible values.

Audio Channel Layout Tags

The identifiers that represent audio channel layouts.

var mNumberChannelDescriptions: UInt32

The number of items in the `mChannelDescriptions` array.

func AudioChannelLayoutTag_GetNumberOfChannels(AudioChannelLayoutTag) -> UInt32

Retrieves the number of channels from an audio channel layout tag.

