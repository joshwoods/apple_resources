

- GameplayKit
- GKGoal
-  init(toStayOn:maxPredictionTime:) 

Initializer

# init(toStayOn:maxPredictionTime:)

Creates a goal whose effect is to maintain an agent’s position within the specified path.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    toStayOn path: GKPath,
    maxPredictionTime: TimeInterval
)
```

## Parameters 

`path`  

A path object.

`maxPredictionTime`  

The amount of time for which to predict an affected agent’s movement.

## Return Value

A new goal object.

## Discussion

This goal uses the shape and the radius property of the specified path to define the boundaries of an area for the agent to stay in. If an affected agent is outside that area, the agent will move into that area; if the agent is already in that area, this goal will not motivate the agent to move further.

The `maxPredictionTime` parameter determines how far ahead of time the agent will predict its own movement to fulfill this goal. For example, with a larger value, an agent moving toward the path will begin to slow gradually so as to stop gently within the path’s radius. With a smaller value, the agent will attempt to stop more abruptly as it reaches the path (and depending on its properties, it might not be able to stop quickly enough to avoid overshooting).

## See Also

### Creating Goals for Path-Following Behavior

convenience init(toFollow: GKPath, maxPredictionTime: TimeInterval, forward: Bool)

Creates a goal whose effect is to both maintain position on and traverse the specified path.

