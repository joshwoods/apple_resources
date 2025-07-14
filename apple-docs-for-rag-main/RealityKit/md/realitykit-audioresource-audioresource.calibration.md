

- RealityKit
- AudioResource
-  AudioResource.Calibration 

Structure

# AudioResource.Calibration

A container for different calibration modes that can be applied for playback.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Calibration
```

## Topics

### Type Methods

static func absolute(dBSPL: Audio.Decibel) -> AudioResource.Calibration

The reference level (-12dBLUFS) of the audio source material will be reproduced at the given `dBSPL` level on known audio output hardware.

static func relative(dBSPL: Audio.Decibel) -> AudioResource.Calibration

Relative adjustment of the resource from the default level of the audio output hardware.

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Audio resources

class AudioFileResource

An audio resource that you load from a file or from a URL.

class AudioFileGroupResource

An audio file group.

class AudioBufferResource

An audio resource that you load from an AVAudioBuffer.

struct AudioLibraryComponent

A container for audio resources that you can look up by user-defined names.

class AudioResource

A playable audio resource

struct Normalization

Normalization adjusts the level of an audio file or buffer to be at a defined target.

