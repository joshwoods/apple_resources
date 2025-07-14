

- GameplayKit
- GKAgent
-  speed 

Instance Property

# speed

The agent’s current forward speed, in units per second.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var speed: Float { get set }
```

## Discussion

This property measures only the agent’s speed in the direction it faces. The concrete subclasses of GKAgent relate speed to orientation and position; see the velocity (GKAgent2D) or velocity (GKAgent3D) property for the appropriate subclass.

