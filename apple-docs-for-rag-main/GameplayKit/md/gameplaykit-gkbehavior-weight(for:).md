

- GameplayKit
- GKBehavior
-  weight(for:) 

Instance Method

# weight(for:)

Returns the weight for the specified goal’s influence on agents.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func weight(for goal: GKGoal) -> Float
```

## Parameters 

`goal`  

A goal already included in the behavior’s set of goals.

## Return Value

The weight to be applied to the goal’s influence on an agent’s speed and direction, or `0.0` if the goal is not in the behavior.

## Discussion

When an agent evaluates its behavior, it examines each goal and calculates the change in direction and speed necessary to move toward fulfilling that goal (within the limits of the current time step and the agent’s maximum speed and turn rate). The agent then combines these influences to determine the total change in direction and speed for the current time step. Weights modulate the effects of multiple goals in a behavior.

## See Also

### Related Documentation

subscript(GKGoal) -> NSNumber!

Returns the weight associated with the goal specified by subscript syntax.

### Managing a Behavior’s Set of Goals

func setWeight(Float, for: GKGoal)

Sets the weight for the specified goal’s influence on agents, adding that goal to the behavior if not already present.

func remove(GKGoal)

Removes the specified goal from the behavior.

func removeAllGoals()

Removes all goals from the behavior.

var goalCount: Int

The number of goals in the behavior.

