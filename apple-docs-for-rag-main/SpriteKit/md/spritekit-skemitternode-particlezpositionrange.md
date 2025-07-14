

- SpriteKit
- SKEmitterNode
-  particleZPositionRange 

Instance Property

# particleZPositionRange

The range of allowed random values for a particle’s depth.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedtvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

**watchOS**

``` source
var particleZPositionRange: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleZPositionRange: CGFloat { get set }
```

## Discussion

The default value is `0.0`. If non-zero, the z position of each particle is randomly determined and may vary by plus or minus half of the range value.

## See Also

### Controlling Particle Position

var particlePosition: CGPoint

The average starting position for a particle.

var particlePositionRange: CGVector

The range of allowed random values for a particle’s position.

var particleZPosition: CGFloat

The average starting depth of a particle.

