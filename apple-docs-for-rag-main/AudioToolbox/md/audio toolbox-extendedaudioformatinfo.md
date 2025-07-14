

- Audio Toolbox
-  ExtendedAudioFormatInfo 

Structure

# ExtendedAudioFormatInfo

A specifier for the kAudioFormatProperty_FormatList property, including the codec to use.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct ExtendedAudioFormatInfo
```

## Topics

### Initializers

init()

init(mASBD: AudioStreamBasicDescription, mMagicCookie: UnsafeRawPointer?, mMagicCookieSize: UInt32, mClassDescription: AudioClassDescription)

### Instance Properties

var mASBD: AudioStreamBasicDescription

A format specification for an audio stream.

var mClassDescription: AudioClassDescription

A structure that describes an audio codec.

var mMagicCookie: UnsafeRawPointer?

Decompression information for the audio data format specified in the `mASBD` field.

var mMagicCookieSize: UInt32

The size, in bytes, of the `mMagicCookie` field.

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

struct AudioPanningInfo

Audio panning information.

typealias AudioFormatPropertyID

A type for four-char codes for audio format property identifiers.

