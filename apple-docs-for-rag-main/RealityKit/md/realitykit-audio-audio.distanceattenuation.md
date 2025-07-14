

- RealityKit
- Audio
-  Audio.DistanceAttenuation 

Enumeration

# Audio.DistanceAttenuation

The different ways that audio intensity diminishes as the distance between the listener and the sound source increases.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum DistanceAttenuation
```

## Topics

### Enumeration Cases

case rolloff(factor: Double)

A standard geometric model for attenuating audio intensity naturally with distance, using a specified loss strength factor.

### Type Properties

static let `default`: Audio.DistanceAttenuation

The default distance attenuation, which uses a rolloff model that mimics real-world physics.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable

## See Also

### Audio types

enum Audio

A namespace for types that are used commonly in audio.

typealias Decibel

The unit for measuring intensity of sound on a logarithmic scale.

enum Directivity

The radiation pattern of sound emitted from an entity.

