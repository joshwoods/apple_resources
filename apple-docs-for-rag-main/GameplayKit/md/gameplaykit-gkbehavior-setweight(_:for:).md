

- GameplayKit
- GKBehavior
-  setWeight(\_:for:) 

Instance Method

# setWeight(\_:for:)

Sets the weight for the specified goal’s influence on agents, adding that goal to the behavior if not already present.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setWeight(
    _ weight: Float,
    for goal: GKGoal
)
```

## Parameters 

`weight`  

A weight to be applied to the goal’s influence on an agent’s speed and direction.

`goal`  

A goal object.

## Discussion

When an agent evaluates its behavior, it examines each goal and calculates the change in direction and speed necessary to move toward fulfilling that goal (within the limits of the current time step and the agent’s maximum speed and turn rate). The agent then combines these influences to determine the total change in direction and speed for the current time step. To modulate the effects of multiple goals in a behavior, use this method to increase or decrease the relative influence of each.

You can use this method to vary the behaviors in your game in response to player actions or other events. For example, an enemy agent’s behavior may combine pursuing the player (init(toInterceptAgent:maxPredictionTime:)) with a bit of wandering (init(toWander:)) to make its movement appear natural. When the enemy has not yet sighted the player, you might reduce the weight of the pursue goal to zero; when the player attacks the enemy, you might increase the weight of the wander goal for a short time to make the enemy act dazed.

## See Also

### Managing a Behavior’s Set of Goals

func weight(for: GKGoal) -> Float

Returns the weight for the specified goal’s influence on agents.

func remove(GKGoal)

Removes the specified goal from the behavior.

func removeAllGoals()

Removes all goals from the behavior.

var goalCount: Int

The number of goals in the behavior.

