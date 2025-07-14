

- Audio Toolbox
-  AudioPanningInfo 

Structure

# AudioPanningInfo

Audio panning information.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioPanningInfo
```

## Topics

### Initializers

init(mPanningMode: AudioPanningMode, mCoordinateFlags: UInt32, mCoordinates: (Float32, Float32, Float32), mGainScale: Float32, mOutputChannelMap: UnsafePointer&lt;AudioChannelLayout>)

### Instance Properties

var mCoordinateFlags: UInt32

For the available coordinate flags, see Channel Coordinate Flags.

var mCoordinates: (Float32, Float32, Float32)

For the available coordinate index constants, see Channel Coordinate Index Constants.

var mGainScale: Float32

A multiplier for audio panning values, typically representing a volume value in the range from 0 to 1. A value of 1 results in audio panning at unity gain. A value of 0 silences all channels.

var mOutputChannelMap: UnsafePointer&lt;AudioChannelLayout>

The channel map used to determine channel volumes for the audio panning.

var mPanningMode: AudioPanningMode

The mode to use for panning.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct AudioBalanceFade

Describes audio left/right balance and front/back fade values.

struct AudioFormatInfo

A structure that specifies an audio format.

struct AudioFormatListItem

struct ExtendedAudioFormatInfo

A specifier for the kAudioFormatProperty_FormatList property, including the codec to use.

typealias AudioFormatPropertyID

A type for four-char codes for audio format property identifiers.

