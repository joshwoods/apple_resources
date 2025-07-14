

- GameplayKit
- GKBehavior
-  init(goal:weight:) 

Initializer

# init(goal:weight:)

Creates a behavior with a single goal.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    goal: GKGoal,
    weight: Float
)
```

## Parameters 

`goal`  

A goal object.

`weight`  

A weight to be applied to the goal’s influence on an agent’s speed and direction.

## Return Value

A new behavior object. To assign a set of goals to an agent, use its behavior property.

## Discussion

For more information, see GameplayKit Programming Guide.

## See Also

### Creating a Behavior

convenience init(goals: [GKGoal])

Creates a behavior with the specified goals.

convenience init(goals: [GKGoal], andWeights: [NSNumber])

Creates a behavior with the specified goals and weights.

convenience init(weightedGoals: [GKGoal : NSNumber])

Creates a behavior with the specified mapping of goals to their weights.

