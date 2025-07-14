

- SpriteKit
-  SKWarpable 

Protocol

# SKWarpable

A protocol for objects that can be warped and animated by an SKWarpGeometry.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
protocol SKWarpable : NSObjectProtocol
```

## Mentioned in 

Animate the Warping of a Sprite

Warping SpriteKit Content By Using an Effect Node

## Topics

### Instance Properties

var subdivisionLevels: Int

The maximum number of subdivision iterations used to generate the final vertices.

**Required**

var warpGeometry: SKWarpGeometry?

The warp geometry used to define the distortion.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- SKEffectNode
- SKScene
- SKSpriteNode

## See Also

### Warping

class SKWarpGeometry

A definition for a deformation of nodes that conform to SKWarpable.

class SKWarpGeometryGrid

A definition for a grid-based deformation of nodes that conform to SKWarpable.

