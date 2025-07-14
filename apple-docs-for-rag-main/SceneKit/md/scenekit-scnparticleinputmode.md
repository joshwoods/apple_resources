

- SceneKit
-  SCNParticleInputMode 

Enumeration

# SCNParticleInputMode

Options for the input value of the property controller’s animation, used by the inputMode property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNParticleInputMode
```

## Topics

### Constants

case overLife

The controller’s effect on a particle property is a function of the time since the particle’s birth.

case overDistance

The controller’s effect on a particle property is a function of the particle’s distance from the position of a specified node.

case overOtherProperty

The controller’s effect on a particle property is a function of another of the particle’s properties.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

