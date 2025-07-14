

- RealityKit
-  AudioFileGroupResource 

Class

# AudioFileGroupResource

An audio file group.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
class AudioFileGroupResource
```

## Topics

### Creating a resource

init([AudioFileResource]) throws

Creates a group resource from an array of audio file resources.

convenience init(named: String, from: String, in: Bundle) async throws

Initializes an audio resource from a Reality Composer Pro project.

static func load(named: String, from: String, in: Bundle?) throws -> AudioFileGroupResource

Loads an audio resource from a Reality Composer Pro project.

### Working with the resource contents

let resources: [AudioFileResource]

The `AudioFileResource` objects which comprise this `AudioFileGroupResource`.

static func == (AudioFileGroupResource, AudioFileGroupResource) -> Bool

### Default Implementations

Hashable Implementations

## Relationships

### Inherits From

- AudioResource

### Conforms To

- Copyable
- Equatable
- Hashable
- Resource
- Sendable

## See Also

### Audio resources

class AudioFileResource

An audio resource that you load from a file or from a URL.

class AudioBufferResource

An audio resource that you load from an AVAudioBuffer.

struct AudioLibraryComponent

A container for audio resources that you can look up by user-defined names.

class AudioResource

A playable audio resource

struct Calibration

A container for different calibration modes that can be applied for playback.

struct Normalization

Normalization adjusts the level of an audio file or buffer to be at a defined target.

