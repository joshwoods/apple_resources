

- RealityKit
-  AudioResource 

Class

# AudioResource

A playable audio resource

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class AudioResource
```

## Topics

### Deprecated

var inputMode: AudioResource.InputModeDeprecated

enum InputModeDeprecated

### Structures

struct Calibration

A container for different calibration modes that can be applied for playback.

struct Normalization

Normalization adjusts the level of an audio file or buffer to be at a defined target.

### Default Implementations

Equatable Implementations

## Relationships

### Inherited By

- AudioBufferResource
- AudioFileGroupResource
- AudioFileResource

### Conforms To

- Copyable
- Equatable
- Resource
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

struct Calibration

A container for different calibration modes that can be applied for playback.

struct Normalization

Normalization adjusts the level of an audio file or buffer to be at a defined target.

