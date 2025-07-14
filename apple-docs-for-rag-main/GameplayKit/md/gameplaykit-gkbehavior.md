

- GameplayKit
-  GKBehavior 

Class

# GKBehavior

A set of goals that together influence the movement of an agent.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKBehavior
```

## Overview

By combining multiple goals (GKGoal objects) you can create complex behavior, such as groups of agents (GKAgent objects) that move together naturally. To assign a set of goals to an agent, use its behavior property.

To learn more about using goals and agents, see Agents, Goals, and Behaviors in GameplayKit Programming Guide.

## Topics

### Creating a Behavior

convenience init(goal: GKGoal, weight: Float)

Creates a behavior with a single goal.

convenience init(goals: [GKGoal])

Creates a behavior with the specified goals.

convenience init(goals: [GKGoal], andWeights: [NSNumber])

Creates a behavior with the specified goals and weights.

convenience init(weightedGoals: [GKGoal : NSNumber])

Creates a behavior with the specified mapping of goals to their weights.

### Managing a Behavior’s Set of Goals

func setWeight(Float, for: GKGoal)

Sets the weight for the specified goal’s influence on agents, adding that goal to the behavior if not already present.

func weight(for: GKGoal) -> Float

Returns the weight for the specified goal’s influence on agents.

func remove(GKGoal)

Removes the specified goal from the behavior.

func removeAllGoals()

Removes all goals from the behavior.

var goalCount: Int

The number of goals in the behavior.

### Working with Goals Using Subscript Syntax

subscript(GKGoal) -> NSNumber!

Returns the weight associated with the goal specified by subscript syntax.

subscript(Int) -> GKGoal

Returns the goal at the specified index in the behavior’s list of goals.

## Relationships

### Inherits From

- NSObject

### Inherited By

- GKCompositeBehavior

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSFastEnumeration
- NSObjectProtocol

## See Also

### Agents, Goals, and Behaviors

class GKAgent

A component that moves a game entity according to a set of goals and realistic constraints.

class GKAgent2D

An agent that operates in a two-dimensional space.

class GKAgent3D

An agent that operates in a three-dimensional space.

class GKGoal

An influence that motivates the movement of one or more agents.

class GKCompositeBehavior

A set of behaviors, each of which is a set of goals, that together influence the movement of an agent.

class GKPath

A polygonal path that can be followed by an agent.

protocol GKAgentDelegate

Implement this protocol to synchronize the state of an agent with its visual representation in your game.

