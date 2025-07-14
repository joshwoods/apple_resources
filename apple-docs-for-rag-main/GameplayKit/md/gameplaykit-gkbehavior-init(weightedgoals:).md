

- GameplayKit
- GKBehavior
-  init(weightedGoals:) 

Initializer

# init(weightedGoals:)

Creates a behavior with the specified mapping of goals to their weights.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(weightedGoals: [GKGoal : NSNumber])
```

## Parameters 

`weightedGoals`  

A dictionary whose keys are goal objects, where each value is the weight to be applied to the corresponding goal’s influence on an agent’s speed and direction.

## Return Value

A new behavior object. To assign a set of goals to an agent, use its behavior property.

## See Also

### Creating a Behavior

convenience init(goal: GKGoal, weight: Float)

Creates a behavior with a single goal.

convenience init(goals: [GKGoal])

Creates a behavior with the specified goals.

convenience init(goals: [GKGoal], andWeights: [NSNumber])

Creates a behavior with the specified goals and weights.

