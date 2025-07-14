

- GameplayKit
- GKCircleObstacle
-  init(radius:) 

Initializer

# init(radius:)

Initializes a circular obstacle with the specified radius.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(radius: Float)
```

## Parameters 

`radius`  

The radius for the new obstacle.

## Return Value

A circular obstacle.

## Discussion

To make agents avoid the obstacle, create a goal with the goalToAvoidObstacles:timeBeforeCollisionToAvoid: method.

For more information, see GameplayKit Programming Guide.

