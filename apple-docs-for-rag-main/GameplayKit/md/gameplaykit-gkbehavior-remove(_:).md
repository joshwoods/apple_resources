

- GameplayKit
- GKBehavior
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the specified goal from the behavior.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func remove(_ goal: GKGoal)
```

## Parameters 

`goal`  

A goal object.

## See Also

### Managing a Behavior’s Set of Goals

func setWeight(Float, for: GKGoal)

Sets the weight for the specified goal’s influence on agents, adding that goal to the behavior if not already present.

func weight(for: GKGoal) -> Float

Returns the weight for the specified goal’s influence on agents.

func removeAllGoals()

Removes all goals from the behavior.

var goalCount: Int

The number of goals in the behavior.

