

- Core Audio Types
-  AudioChannelLayoutTag_GetNumberOfChannels(\_:) 

Function

# AudioChannelLayoutTag_GetNumberOfChannels(\_:)

Retrieves the number of channels from an audio channel layout tag.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func AudioChannelLayoutTag_GetNumberOfChannels(_ inLayoutTag: AudioChannelLayoutTag) -> UInt32
```

## Parameters 

`inLayoutTag`  

The layout tag from which to retrieve the number of channels.

## Return Value

A count of audio channels.

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

typealias AudioChannelLayoutTag

Identifies a previously-defined channel layout.

Audio Channel Layout Tags

The identifiers that represent audio channel layouts.

var mNumberChannelDescriptions: UInt32

The number of items in the `mChannelDescriptions` array.

