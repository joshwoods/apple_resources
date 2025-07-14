

- GameplayKit
- GKBehavior
-  init(goals:andWeights:) 

Initializer

# init(goals:andWeights:)

Creates a behavior with the specified goals and weights.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    goals: [GKGoal],
    andWeights weights: [NSNumber]
)
```

## Parameters 

`goals`  

An array of goal objects.

`weights`  

An array of numbers, each the weight to be applied to the goal at the corresponding index in the `goals` array.

## Return Value

A new behavior object. To assign a set of goals to an agent, use its behavior property.

## See Also

### Creating a Behavior

convenience init(goal: GKGoal, weight: Float)

Creates a behavior with a single goal.

convenience init(goals: [GKGoal])

Creates a behavior with the specified goals.

convenience init(weightedGoals: [GKGoal : NSNumber])

Creates a behavior with the specified mapping of goals to their weights.

