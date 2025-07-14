

- RealityKit
- AudioBufferResource
-  AudioBufferResource.Configuration 

Structure

# AudioBufferResource.Configuration

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Configuration
```

## Topics

### Initializers

init(shouldLoop: Bool, shouldRandomizeStartTime: Bool, normalization: AudioResource.Normalization?, calibration: AudioResource.Calibration?, mixGroupName: String?)

### Instance Properties

var calibration: AudioResource.Calibration?

var mixGroupName: String?

var normalization: AudioResource.Normalization?

var shouldLoop: Bool

var shouldRandomizeStartTime: Bool

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

