

- SpriteKit
- SKAction
-  warp(to:duration:) 

Type Method

# warp(to:duration:)

Creates an action to distort a node based using an SKWarpGeometry object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class func warp(
    to warp: SKWarpGeometry,
    duration: TimeInterval
) -> SKAction?
```

## Parameters 

`warp`  

The warp geometry to distort the node to.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Mentioned in 

Animate the Warping of a Sprite

## Discussion

The numberOfColumns and numberOfRows in the node’s current geometry should match those of the specified geometry.

## See Also

### Animate the Warping of a Node

class func animate(withWarps: [SKWarpGeometry], times: [NSNumber]) -> SKAction?

Creates an action to distort a node through a sequence of SKWarpGeometry objects.

class func animate(withWarps: [SKWarpGeometry], times: [NSNumber], restore: Bool) -> SKAction?

Creates an action to distort a node through a sequence of SKWarpGeometry objects.

