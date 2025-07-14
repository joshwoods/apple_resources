

- SpriteKit
- SKFieldNode
-  smoothness 

Instance Property

# smoothness

The smoothness of the noise used to generate the forces.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var smoothness: Float { get set }
```

**watchOS**

``` source
var smoothness: Float { get set }
```

## Discussion

This parameter should be a value between `0.0` and `1.0`, where `1.0` represents a uniform smoothness.

## See Also

### Configuring Other Field Properties

var animationSpeed: Float

The rate at which a noise or turbulence field node changes.

var direction: vector_float3

The direction of a velocity field node.

var texture: SKTexture?

A normal texture that specifies the velocities at different points in a velocity field node.

