

- GameplayKit
- GKAgent
-  mass 

Instance Property

# mass

The resistance of the agent to changes in speed or direction.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var mass: Float { get set }
```

## Discussion

The higher the value of this property, the slower the agent will be to respond to goals that change its speed or direction, and vice versa.

Note

The simulation responsible for agent movement is based on realistic physical behaviors; however, this simulation is *not* connected to the physics subsystems in SpriteKit, SceneKit, or any other graphics engine. For example, setting the mass property of an agent does not affect the collision behavior of any SpriteKit physics bodies.

## See Also

### Constraining an Agent’s Movement

var maxAcceleration: Float

The upper limit to changes in the agent’s speed or direction.

var maxSpeed: Float

The agent’s maximum forward speed, in units per second.

var radius: Float

The agent’s radius.

