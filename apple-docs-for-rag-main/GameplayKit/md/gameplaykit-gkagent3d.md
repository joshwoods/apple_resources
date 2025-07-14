

- GameplayKit
-  GKAgent3D 

Class

# GKAgent3D

An agent that operates in a three-dimensional space.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKAgent3D
```

## Overview

Agents are game entities that move according to realistic constraints and whose behavior is determined by goals that motivate movement. The general functionality of an agent is defined by the abstract superclass GKAgent; however, you use instances of the GKAgent3D class to implement agent-based gameplay in a 3D game.

To learn more about using goals and agents, see Agents, Goals, and Behaviors in GameplayKit Programming Guide.

## Topics

### Managing an Agent’s Position and Orientation

var position: vector_float3

The current position of the agent in 3D space.

var rotation: matrix_float3x3

The orientation of the agent in 3D space.

### Running the Agent Simulation

func update(deltaTime: TimeInterval)

Causes the agent to evaluate its goals and update its position, rotation, and velocity accordingly.

var velocity: vector_float3

The current velocity of the agent in 3D space.

### Instance Properties

var rightHanded: Bool

## Relationships

### Inherits From

- GKAgent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Agents, Goals, and Behaviors

class GKAgent

A component that moves a game entity according to a set of goals and realistic constraints.

class GKAgent2D

An agent that operates in a two-dimensional space.

class GKGoal

An influence that motivates the movement of one or more agents.

class GKBehavior

A set of goals that together influence the movement of an agent.

class GKCompositeBehavior

A set of behaviors, each of which is a set of goals, that together influence the movement of an agent.

class GKPath

A polygonal path that can be followed by an agent.

protocol GKAgentDelegate

Implement this protocol to synchronize the state of an agent with its visual representation in your game.

