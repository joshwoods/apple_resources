

- RealityKit
- AudioResource
-  AudioResource.Normalization 

Structure

# AudioResource.Normalization

Normalization adjusts the level of an audio file or buffer to be at a defined target.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Normalization
```

## Overview

Audio files produced in a production environment where dynamics are already being processed may not need normalization.

Normalization has a CPU cost on *load* for audio file resources that have a loading strategy of AudioFileResource.LoadingStrategy.preload and a CPU cost on *playback* for audio files that have a loading strategy of AudioFileResource.LoadingStrategy.stream.

## Topics

### Type Properties

static let dynamic: AudioResource.Normalization

Performs dynamic compression to normalize the audio source material to a level of -12dBLUFS in real-time.

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

struct Calibration

A container for different calibration modes that can be applied for playback.

