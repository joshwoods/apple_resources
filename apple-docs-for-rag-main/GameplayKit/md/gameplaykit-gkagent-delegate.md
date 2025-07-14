

- GameplayKit
- GKAgent
-  delegate 

Instance Property

# delegate

An object that prepares for or responds to updates in the agent simulation.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
weak var delegate: (any GKAgentDelegate)? { get set }
```

## Discussion

When you call the agent’s update(deltaTime:) method (directly or through an entity or component system), the agent sends messages to its delegate before and after evaluating its goals and updating its position and direction to match. You can use the methods in the GKAgentDelegate protocol to update the visual representation of an agent, or to change the agent’s position and direction based on external influences such as a SpriteKit or SceneKit physics simulation.

