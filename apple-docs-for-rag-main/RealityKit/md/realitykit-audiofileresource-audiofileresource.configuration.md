

- RealityKit
- AudioFileResource
-  AudioFileResource.Configuration 

Structure

# AudioFileResource.Configuration

A container for various settings for loading an audio file resource.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Configuration
```

## Topics

### Creating a configuration for an audio file resource

init(loadingStrategy: AudioFileResource.LoadingStrategy, shouldLoop: Bool, shouldRandomizeStartTime: Bool, normalization: AudioResource.Normalization?, calibration: AudioResource.Calibration?, mixGroupName: String?)

Initializes a new audio file resource configuration.

### Configuring the loading optimization strategy

var loadingStrategy: AudioFileResource.LoadingStrategy

Stores the strategy the system uses for handling an audio resource’s data before and during playback.

### Controlling the volume

var normalization: AudioResource.Normalization?

Stores the normalization portion of the configuration.

var calibration: AudioResource.Calibration?

Stores the calibration setting that the system applies to the audio resource, ensuring optimal playback quality.

### Customizing the playback

var shouldRandomizeStartTime: Bool

Stores a Boolean indicating whether the playback begins from the start of the file, or from a random position.

var shouldLoop: Bool

Stores a Boolean indicating whether the playback loops infinitely, until manually stopped or paused.

### Assigning an audio resource to a mix group

var mixGroupName: String?

An arbitrary name that can assigns an audio resource to an audio mix group.

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

### Supporting types

enum LoadingStrategy

A container for different strategies on how to handle resources’ data before and during playback.

