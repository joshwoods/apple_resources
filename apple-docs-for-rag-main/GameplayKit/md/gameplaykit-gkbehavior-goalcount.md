

- GameplayKit
- GKBehavior
-  goalCount 

Instance Property

# goalCount

The number of goals in the behavior.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var goalCount: Int { get }
```

## See Also

### Managing a Behavior’s Set of Goals

func setWeight(Float, for: GKGoal)

Sets the weight for the specified goal’s influence on agents, adding that goal to the behavior if not already present.

func weight(for: GKGoal) -> Float

Returns the weight for the specified goal’s influence on agents.

func remove(GKGoal)

Removes the specified goal from the behavior.

func removeAllGoals()

Removes all goals from the behavior.

