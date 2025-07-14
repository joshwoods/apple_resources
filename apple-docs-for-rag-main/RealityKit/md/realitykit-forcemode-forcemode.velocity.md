

- RealityKit
- ForceMode
-  ForceMode.velocity 

Case

# ForceMode.velocity

A direct adjustment to a body’s linear or angular velocity, independent of its mass or inertia.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case velocity
```

## Discussion

The quantity that user sets via setForce(_:index:) has the units of distance / time. `velocity` mode causes a change in velocity independent of a body’s mass.

The quantity that user sets via setTorque(_:index:) has the units of 1 / time or radian / time. `velocity` mode causes a change in angular velocity independent of a body’s mass or inertia.

