

- GameplayKit
- GKAgent2D
-  velocity 

Instance Property

# velocity

The current velocity of the agent in 2D space.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var velocity: vector_float2 { get }
```

## Discussion

An agent’s velocity is a calculated property—the velocity vector is determined by an agent’s facing direction (its rotation property) and its speed property.

## See Also

### Running the Agent Simulation

func update(deltaTime: TimeInterval)

Causes the agent to evaluate its goals and update its position, rotation, and velocity accordingly.

