

- SpriteKit
- SKAction
-  scale(to:duration:) 

Type Method

# scale(to:duration:)

Creates an action that changes the x and y scale values of a node to achieve

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class func scale(
    to size: CGSize,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`size`  

The new size of the node.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s xScale and yScale properties are animated to achieve the specified size in its parent’s coordinate space.

This action is not reversible; the reverse of this action has the same duration but does not change anything.

## See Also

### Animating the Scaling of a Node

class func scale(by: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node by a relative value.

class func scale(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node.

class func scaleX(by: CGFloat, y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that adds relative values to the x and y scale values of a node.

class func scaleX(to: CGFloat, y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node.

class func scaleX(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x scale value of a node to a new value.

class func scaleY(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the y scale value of a node to a new value.

