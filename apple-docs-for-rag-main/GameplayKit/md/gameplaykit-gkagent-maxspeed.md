

- GameplayKit
- GKAgent
-  maxSpeed 

Instance Property

# maxSpeed

The agent’s maximum forward speed, in units per second.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var maxSpeed: Float { get set }
```

## Discussion

When an agent evaluates the goals listed in its behavior property, the result is an acceleration vector that changes the velocity of the agent. If the magnitude of the new velocity is greater than this value, the velocity is reduced to match this value.

## See Also

### Related Documentation

var speed: Float

The agent’s current forward speed, in units per second.

### Constraining an Agent’s Movement

var mass: Float

The resistance of the agent to changes in speed or direction.

var maxAcceleration: Float

The upper limit to changes in the agent’s speed or direction.

var radius: Float

The agent’s radius.

