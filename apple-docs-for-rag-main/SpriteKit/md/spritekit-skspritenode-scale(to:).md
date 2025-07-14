

- SpriteKit
- SKSpriteNode
-  scale(to:) 

Instance Method

# scale(to:)

Scales the sprite node to a specified size.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
func scale(to size: CGSize)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func scale(to size: CGSize)
```

## Discussion

This method works by setting the sprite node’s xScale and yScale to achieve the specified size in its parent’s coordinate space.

## See Also

### Setting a Sprite’s Size and Position

Using the Anchor Point to Move a Sprite

Learn how the anchor point affects a sprite’s position.

var size: CGSize

The dimensions of the sprite, in points.

var anchorPoint: CGPoint

Defines the point in the sprite that corresponds to the node’s position.

