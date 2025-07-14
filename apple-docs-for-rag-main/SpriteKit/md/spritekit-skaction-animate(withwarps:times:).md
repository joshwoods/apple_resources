

- SpriteKit
- SKAction
-  animate(withWarps:times:) 

Type Method

# animate(withWarps:times:)

Creates an action to distort a node through a sequence of SKWarpGeometry objects.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class func animate(
    withWarps warps: [SKWarpGeometry],
    times: [NSNumber]
) -> SKAction?
```

## Parameters 

`warps`  

The sequence of warps to apply to the node.

`times`  

The times at which each warp distortion in the sequence should complete.

## Return Value

A new action object.

## Mentioned in 

Animate the Warping of a Sprite

## Discussion

The numberOfColumns and numberOfRows in each geometry in the sequence should match.

## See Also

### Animate the Warping of a Node

class func animate(withWarps: [SKWarpGeometry], times: [NSNumber], restore: Bool) -> SKAction?

Creates an action to distort a node through a sequence of SKWarpGeometry objects.

class func warp(to: SKWarpGeometry, duration: TimeInterval) -> SKAction?

Creates an action to distort a node based using an SKWarpGeometry object.

