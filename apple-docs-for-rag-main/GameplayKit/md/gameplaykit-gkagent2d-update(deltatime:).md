

- GameplayKit
- GKAgent2D
-  update(deltaTime:) 

Instance Method

# update(deltaTime:)

Causes the agent to evaluate its goals and update its position, rotation, and velocity accordingly.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func update(deltaTime seconds: TimeInterval)
```

## Discussion

You call this method directly on an individual agent, or on all the agents in your game through a GKComponentSystem object, whenever you want to run a step of the agent simulation. Typically, a game updates its agent simulation whenever it prepares to draw a new frame—for example, in the update(_:) method of a SpriteKit SKScene object.

## See Also

### Running the Agent Simulation

var velocity: vector_float2

The current velocity of the agent in 2D space.

