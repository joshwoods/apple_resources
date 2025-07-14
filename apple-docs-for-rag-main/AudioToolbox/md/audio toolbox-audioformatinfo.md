

- Audio Toolbox
-  AudioFormatInfo 

Structure

# AudioFormatInfo

A structure that specifies an audio format.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioFormatInfo
```

## Overview

Use this value with the kAudioFormatProperty_FormatList property.

## Topics

### Initializers

init(mASBD: AudioStreamBasicDescription, mMagicCookie: UnsafeRawPointer, mMagicCookieSize: UInt32)

### Instance Properties

var mASBD: AudioStreamBasicDescription

An `AudioStreamBasicDescription` structure.

var mMagicCookie: UnsafeRawPointer

A pointer to the decompression information for the data described in the `mASBD` parameter.

var mMagicCookieSize: UInt32

The size, in bytes, of the `mMagicCookie` parameter.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct AudioBalanceFade

Describes audio left/right balance and front/back fade values.

struct AudioFormatListItem

struct AudioPanningInfo

Audio panning information.

struct ExtendedAudioFormatInfo

A specifier for the kAudioFormatProperty_FormatList property, including the codec to use.

typealias AudioFormatPropertyID

A type for four-char codes for audio format property identifiers.

