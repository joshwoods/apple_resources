

- GameplayKit
- GKGoal
-  init(toFleeAgent:) 

Initializer

# init(toFleeAgent:)

Creates a goal whose effect is to move an agent away from the current position of the specified other agent.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(toFleeAgent agent: GKAgent)
```

## Parameters 

`agent`  

An agent whose position affected agents will attempt to move away from.

## Return Value

A new goal object.

## Discussion

This goal is similar to one produced by the init(toAvoid:maxPredictionTime:) method with a single agent and a `maxPredictionTime` parameter of zero. Affected agents will attempt to move away from the target agent, but without taking the target’s movement into account.

You can also use this goal when you want an agent to move away from a target point, such as the current mouse or touch location. Create another agent that remains stationary at the target point (that is, has no velocity and no goals), and use that agent as the parameter when creating a goal with this method.

## See Also

### Creating Goals for General Movement Behavior

convenience init(toSeekAgent: GKAgent)

Creates a goal whose effect is to move an agent toward the current position of the specified other agent.

convenience init(toReachTargetSpeed: Float)

Creates a goal whose effect is to accelerate or decelerate an agent until it reaches the specified speed.

convenience init(toWander: Float)

Creates a goal whose effect is to make an agent wander aimlessly, moving forward and turning at random.

