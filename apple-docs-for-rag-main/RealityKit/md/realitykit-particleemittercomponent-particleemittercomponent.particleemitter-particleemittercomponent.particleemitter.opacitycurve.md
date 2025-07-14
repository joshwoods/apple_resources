

- RealityKit
- ParticleEmitterComponent
- ParticleEmitterComponent.ParticleEmitter
-  ParticleEmitterComponent.ParticleEmitter.OpacityCurve 

Enumeration

# ParticleEmitterComponent.ParticleEmitter.OpacityCurve

Options for the curve of opacity change over the lifetime of the particle, used by the opacityOverLife property.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum OpacityCurve
```

## Topics

### Operators

static func == (ParticleEmitterComponent.ParticleEmitter.OpacityCurve, ParticleEmitterComponent.ParticleEmitter.OpacityCurve) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case constant

case easeFadeIn

case easeFadeOut

case gradualFadeInOut

case linearFadeIn

case linearFadeOut

case quickFadeInOut

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable

