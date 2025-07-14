

- SpriteKit
- SKEmitterNode
-  particleLifetimeRange 

Instance Property

# particleLifetimeRange

The range of allowed random values for a particle’s lifetime.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleLifetimeRange: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleLifetimeRange: CGFloat { get set }
```

## Discussion

The default value is `0.0`. If non-zero, the lifetime of each particle is randomly determined and may vary by plus or minus half of the range value.

## See Also

### Controlling Particle Lifetime

var particleLifetime: CGFloat

The average lifetime of a particle, in seconds.

