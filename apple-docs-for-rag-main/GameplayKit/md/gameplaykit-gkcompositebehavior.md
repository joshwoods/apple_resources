

- GameplayKit
-  GKCompositeBehavior 

Class

# GKCompositeBehavior

A set of behaviors, each of which is a set of goals, that together influence the movement of an agent.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKCompositeBehavior
```

## Overview

By composing GKGoal objects into subgroups (GKBehavior objects) and composing those behaviors into composite behaviors, you can control certain aspects of a GKAgent object’s movement in concert. To assign a behavior to an agent, use its behavior property.

For example, you might create a behavior for a set of agents to stay together as a flock (with cohesion, alignment, and separation goals) while loosely following a path. With a single GKBehavior object, whenever you want to change the importance of the flocking goals relative to the path-following goals, you’d need to individually change the weight of each goal. With a composite behavior, you can adjust the relative influence of a group of goals together, as in the following code.

- Swift
- Objective-C

```
```

```
```

After constructing this behavior, you can use the setWeight(_:for:) method to increase or decrease the influence of the `flock` and `meanderOnPath` behaviors relative to one another.

To learn more about using goals and agents, see Agents, Goals, and Behaviors in GameplayKit Programming Guide.

## Topics

### Creating a Composite Behavior

convenience init(behaviors: [GKBehavior])

Creates a composite behavior from the specified individual behaviors.

convenience init(behaviors: [GKBehavior], andWeights: [NSNumber])

Creates a behavior with the specified behaviors and weights.

### Managing the Individual Behaviors in a Composite Behavior

func setWeight(Float, for: GKBehavior)

Sets the weight for the specified individual behavior’s influence on agents, adding that behavior to the composite behavior if it is not already present.

func weight(for: GKBehavior) -> Float

Returns the weight for the specified individual behavior’s influence on agents.

func remove(GKBehavior)

Removes the specified individual behavior from the composite behavior.

func removeAllBehaviors()

Removes all individual behaviors from the composite behavior.

var behaviorCount: Int

The number of individual behaviors in the composite behavior.

### Working with Behaviors Using Subscript Syntax

subscript(GKBehavior) -> NSNumber

Returns the weight associated with the behavior specified by subscript syntax.

subscript(Int) -> GKBehavior

Returns the individual behavior at the specified index in the composite behavior’s list of behaviors.

## Relationships

### Inherits From

- GKBehavior

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

class GKBehavior

A set of goals that together influence the movement of an agent.

class GKPath

A polygonal path that can be followed by an agent.

protocol GKAgentDelegate

Implement this protocol to synchronize the state of an agent with its visual representation in your game.

