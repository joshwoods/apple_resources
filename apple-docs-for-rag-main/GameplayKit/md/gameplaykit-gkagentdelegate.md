

- GameplayKit
-  GKAgentDelegate 

Protocol

# GKAgentDelegate

Implement this protocol to synchronize the state of an agent with its visual representation in your game.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol GKAgentDelegate : NSObjectProtocol
```

## Overview

A GKAgent object simulates its own movement according to constraints and goals. Use this protocol to manage an external object related to the agent, such as the sprite or 3D object that provides that agent’s visual representation in your game.

You can synchronize with an agent in either or both directions:

- To update a visual representation based on the latest data from the agent simulation, implement the agentDidUpdate(_:) method. In this method you can read the position and rotation properties of the agent (as a GKAgent2D or GKAgent3D object) and set the corresponding attributes of whatever object provides the agent’s visual representation.

- To update the agent simulation with data from an external source—for example, if the game object corresponding to an agent is also affected by a physics engine such as those used in SpriteKit and SceneKit—implement the agentWillUpdate(_:) method. In this method you can set the position and rotation properties of the agent (as a GKAgent2D or GKAgent3D object) so that the next simulation step will take your changes to those properties into account.

Tip

If you use the GKSKNodeComponent class to manage the relationship between an entity and a SpriteKit node, set your GKSKNodeComponent instance as the delegate for that entity’s agent, and GameplayKit will automatically synchronize the agent and its SpriteKit representation.

To learn more about using goals and agents, see Agents, Goals, and Behaviors in GameplayKit Programming Guide.

## Topics

### Synchronizing with Agents

func agentWillUpdate(GKAgent)

Tells the delegate that an agent is about to perform its next simulation step.

func agentDidUpdate(GKAgent)

Tells the delegate that an agent has just performed a simulation step.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- GKSCNNodeComponent
- GKSKNodeComponent

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

class GKCompositeBehavior

A set of behaviors, each of which is a set of goals, that together influence the movement of an agent.

class GKPath

A polygonal path that can be followed by an agent.

