

- GameplayKit
- GKGoal
-  init(toWander:) 

Initializer

# init(toWander:)

Creates a goal whose effect is to make an agent wander aimlessly, moving forward and turning at random.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(toWander speed: Float)
```

## Parameters 

`speed`  

The forward speed for affected agents to maintain while turning at random.

## Return Value

A new goal object.

## See Also

### Creating Goals for General Movement Behavior

convenience init(toSeekAgent: GKAgent)

Creates a goal whose effect is to move an agent toward the current position of the specified other agent.

convenience init(toFleeAgent: GKAgent)

Creates a goal whose effect is to move an agent away from the current position of the specified other agent.

convenience init(toReachTargetSpeed: Float)

Creates a goal whose effect is to accelerate or decelerate an agent until it reaches the specified speed.

