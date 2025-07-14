

- SpriteKit
- SKReachConstraints
-  init(lowerAngleLimit:upperAngleLimit:) 

Initializer

# init(lowerAngleLimit:upperAngleLimit:)

Initializes a new reach constraint object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(
    lowerAngleLimit: CGFloat,
    upperAngleLimit: CGFloat
)
```

## Parameters 

`lowerAngleLimit`  

The minimum angle that the node can have when it is rotated by a reach event.

`upperAngleLimit`  

The maximum angle that the node can have when it is rotated by a reach event.

## Return Value

A newly initialized reach constraint.

## Discussion

When a reach action is executed, a node’s zRotation property may be changed by the action to satisfy the reach action. Any value calculated by the reach action for a node is always inside the range specified by the reach constraint attached to the node’s reachConstraints property.

## See Also

### Working with Reach Constraints

var lowerAngleLimit: CGFloat

The minimum angle that the node can have after it is rotated by a reach event.

var upperAngleLimit: CGFloat

The maximum angle that the node can have after it is rotated by a reach event.

