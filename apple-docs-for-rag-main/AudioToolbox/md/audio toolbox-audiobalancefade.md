

- Audio Toolbox
-  AudioBalanceFade 

Structure

# AudioBalanceFade

Describes audio left/right balance and front/back fade values.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioBalanceFade
```

## Overview

This data structure is used with the kAudioFormatProperty_BalanceFade property.

## Topics

### Initializers

init(mLeftRightBalance: Float32, mBackFrontFade: Float32, mType: AudioBalanceFadeType, mChannelLayout: UnsafePointer&lt;AudioChannelLayout>)

### Instance Properties

var mBackFrontFade: Float32

The audio front/back fade, where -1 represents full rear, 0 represents center, and +1 represents full front.

var mChannelLayout: UnsafePointer&lt;AudioChannelLayout>

The size, in bytes, of the `mMagicCookie` parameter.

var mLeftRightBalance: Float32

The audio left/right balance, where -1 represents full left, 0 represents center, and +1 represents full right.

var mType: AudioBalanceFadeType

An AudioBalanceFadeType constant. max unity gain, or equal power.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct AudioFormatInfo

A structure that specifies an audio format.

struct AudioFormatListItem

struct AudioPanningInfo

Audio panning information.

struct ExtendedAudioFormatInfo

A specifier for the kAudioFormatProperty_FormatList property, including the codec to use.

typealias AudioFormatPropertyID

A type for four-char codes for audio format property identifiers.

