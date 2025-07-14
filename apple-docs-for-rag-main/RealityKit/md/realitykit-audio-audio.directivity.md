

- RealityKit
- Audio
-  Audio.Directivity 

Enumeration

# Audio.Directivity

The radiation pattern of sound emitted from an entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum Directivity
```

## Topics

### Enumeration Cases

case beam(focus: Double)

A parametric frequency-dependent radiation pattern, where the `focus` determines the width of a beam.

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

enum DistanceAttenuation

The different ways that audio intensity diminishes as the distance between the listener and the sound source increases.

