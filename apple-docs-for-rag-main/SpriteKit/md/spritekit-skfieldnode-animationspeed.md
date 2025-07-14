

- SpriteKit
- SKFieldNode
-  animationSpeed 

Instance Property

# animationSpeed

The rate at which a noise or turbulence field node changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
var animationSpeed: Float { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var animationSpeed: Float { get set }
```

## Discussion

A value of `0.0` means that the field should not animate at all.

## See Also

### Configuring Other Field Properties

var smoothness: Float

The smoothness of the noise used to generate the forces.

var direction: vector_float3

The direction of a velocity field node.

var texture: SKTexture?

A normal texture that specifies the velocities at different points in a velocity field node.

