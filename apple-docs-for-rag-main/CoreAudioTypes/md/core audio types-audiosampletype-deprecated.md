

- Core Audio Types
-  AudioSampleType Deprecated

Type Alias

# AudioSampleType

The canonical audio data sample type for input and output.

iOS 2.0+iPadOS 2.0+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 3.0+

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
typealias AudioSampleType = Int16
```

**Mac Catalyst, macOS**

``` source
typealias AudioSampleType = Float32
```

Deprecated

The concept of canonical formats is deprecated

## Discussion

The canonical audio sample type for input and output in iPhone OS is linear PCM with 16-bit integer samples.

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

typealias AudioUnitSampleType

The canonical audio data sample type for audio processing.

Deprecated

struct AudioFormatListItem

