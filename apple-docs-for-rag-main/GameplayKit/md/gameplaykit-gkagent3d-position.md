

- GameplayKit
- GKAgent3D
-  position 

Instance Property

# position

The current position of the agent in 3D space.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var position: vector_float3 { get set }
```

## Discussion

The agent updates its own position, rotation, and velocity according to its goals when you call its update(deltaTime:) method.

However, you can still directly change the position of an agent. Do this when you want to set the position of a static agent (that is, one with no goals) or move an agent as a direct result of user input. For example, to make a game character follow a touch (in iOS) or the mouse pointer (in macOS), you can create an invisible agent and continually update that agent’s position to match that of the touch or mouse event. Then, give the agent representing the game character a goal created with the init(toSeekAgent:) method, targeting the invisible agent.

For more information, see GameplayKit Programming Guide.

## See Also

### Managing an Agent’s Position and Orientation

var rotation: matrix_float3x3

The orientation of the agent in 3D space.

