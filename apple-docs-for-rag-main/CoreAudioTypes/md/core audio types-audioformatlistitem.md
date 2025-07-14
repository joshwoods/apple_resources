

- Core Audio Types
-  AudioFormatListItem 

Structure

# AudioFormatListItem

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct AudioFormatListItem
```

## Overview

```
@struct     AudioFormatListItem
@abstract   this struct is used as output from the kAudioFormatProperty_FormatList property
@var        mASBD
                an AudioStreamBasicDescription
@var        mChannelLayoutTag
                an AudioChannelLayoutTag
```

## Topics

### Initializers

init()

init(mASBD: AudioStreamBasicDescription, mChannelLayoutTag: AudioChannelLayoutTag)

### Instance Properties

var mASBD: AudioStreamBasicDescription

var mChannelLayoutTag: AudioChannelLayoutTag

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Common Types

typealias AVAudioInteger

An integer type for audio operations.

typealias AVAudioUInteger

An unsigned integer type for audio operations.

typealias AudioSessionID

A unique identifier of an audio session.

var kAudioUnitSampleFractionBits: Int32

The number of fractional bits in fixed-point samples.

var COREAUDIOTYPES_VERSION: Int32

A value that represents the Core Audio Types version.

typealias AudioSampleType

The canonical audio data sample type for input and output.

Deprecated

typealias AudioUnitSampleType

The canonical audio data sample type for audio processing.

Deprecated

