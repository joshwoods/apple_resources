

- GameplayKit
- GKSphereObstacle
-  init(radius:) 

Initializer

# init(radius:)

Initializes a spherical obstacle with the specified radius.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
init(radius: Float)
```

## Parameters 

`radius`  

The radius for the new obstacle.

## Return Value

A spherical obstacle.

## Discussion

To make agents avoid the obstacle, create a goal with the goalToAvoidObstacles:timeBeforeCollisionToAvoid: method.

