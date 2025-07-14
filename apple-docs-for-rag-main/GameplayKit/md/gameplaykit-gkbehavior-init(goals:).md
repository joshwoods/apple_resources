

- GameplayKit
- GKBehavior
-  init(goals:) 

Initializer

# init(goals:)

Creates a behavior with the specified goals.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(goals: [GKGoal])
```

## Parameters 

`goals`  

An array of goal objects.

## Return Value

A new behavior object. To assign a set of goals to an agent, use its behavior property.

## Discussion

The new behavior contains the specified goals, each with a weight of `1.0`. To change a goal’s weight after creating the behavior, keep a reference to that goal and use the setWeight(_:for:) method.

## See Also

### Creating a Behavior

convenience init(goal: GKGoal, weight: Float)

Creates a behavior with a single goal.

convenience init(goals: [GKGoal], andWeights: [NSNumber])

Creates a behavior with the specified goals and weights.

convenience init(weightedGoals: [GKGoal : NSNumber])

Creates a behavior with the specified mapping of goals to their weights.

