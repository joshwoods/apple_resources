

- RealityKit
- ForceMode
-  ForceMode.impulse 

Case

# ForceMode.impulse

A direct adjustment to a body’s linear or angular momentum.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case impulse
```

## Discussion

The quantity that user sets via setForce(_:index:) has the units of mass \* distance / time. `impulse` mode causes a change in linear momentum.

The quantity that user sets via setTorque(_:index:) has the units of mass \* distance^2 / time. `impulse` mode causes a change in angular momentum.

