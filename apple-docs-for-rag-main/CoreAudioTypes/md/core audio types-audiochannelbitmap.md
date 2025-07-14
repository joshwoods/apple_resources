

- Core Audio Types
-  AudioChannelBitmap 

Structure

# AudioChannelBitmap

The supported channel bitmaps to use when defining channel layouts.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
struct AudioChannelBitmap
```

## Topics

### Left

static var bit_Left: AudioChannelBitmap

The left channel.

static var bit_LeftCenter: AudioChannelBitmap

The left center channel.

static var bit_LeftSurround: AudioChannelBitmap

The left surround channel.

static var bit_LeftSurroundDirect: AudioChannelBitmap

The left surround direct channel.

static var bit_LeftTopFront: AudioChannelBitmap

The left-top front channel.

static var bit_LeftTopMiddle: AudioChannelBitmap

The left-top middle channel.

static var bit_LeftTopRear: AudioChannelBitmap

The left-top rear channel.

static var bit_TopBackLeft: AudioChannelBitmap

The top-back left channel.

static var bit_VerticalHeightLeft: AudioChannelBitmap

The vertical height left channel.

### Center

static var bit_Center: AudioChannelBitmap

The center channel.

static var bit_CenterSurround: AudioChannelBitmap

The center surround channel.

static var bit_CenterTopFront: AudioChannelBitmap

The top-front center channel.

static var bit_CenterTopMiddle: AudioChannelBitmap

The top-middle center channel.

static var bit_CenterTopRear: AudioChannelBitmap

The top-right center channel.

static var bit_TopBackCenter: AudioChannelBitmap

The top-back center channel.

static var bit_TopCenterSurround: AudioChannelBitmap

The top center surround channel.

static var bit_VerticalHeightCenter: AudioChannelBitmap

The vertical height center channel.

### Right

static var bit_Right: AudioChannelBitmap

The right channel.

static var bit_RightCenter: AudioChannelBitmap

The right center channel.

static var bit_RightSurround: AudioChannelBitmap

The rIght surround channel.

static var bit_RightSurroundDirect: AudioChannelBitmap

The right surround direct channel.

static var bit_RightTopFront: AudioChannelBitmap

The top-front front channel.

static var bit_RightTopMiddle: AudioChannelBitmap

The top-middle right channel.

static var bit_RightTopRear: AudioChannelBitmap

The top-rear right channel.

static var bit_TopBackRight: AudioChannelBitmap

The top-back right channel.

static var bit_VerticalHeightRight: AudioChannelBitmap

The vertical height right channel.

### Low-Frequency Effects

static var bit_LFEScreen: AudioChannelBitmap

The Low Frequency Effects (LFE) screen channel.

### Initializers

init(rawValue: UInt32)

Creates an audio channel bitmap.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Accessing the Data

var mChannelBitmap: AudioChannelBitmap

If `mChannelLayoutTag` is set to `kAudioChannelLayoutTag_UseChannelBitmap`, this field is the channel-use bitmap.

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

func AudioChannelLayoutTag_GetNumberOfChannels(AudioChannelLayoutTag) -> UInt32

Retrieves the number of channels from an audio channel layout tag.

