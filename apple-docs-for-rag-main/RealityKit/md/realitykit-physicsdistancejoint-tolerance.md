

- RealityKit
- PhysicsDistanceJoint
-  tolerance 

Instance Property

# tolerance

An extension of the distance limit, as a percentage-based error tolerance.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var tolerance: Float
```

## Discussion

For example, a tolerance of `0.01` extends the distance limit by `1` percent. When the pins exceed this distance, the joint constrains the pins until they are within the distance limit.

Important

Use a non-negative value for the tolerance.

