

- RealityKit
- ForceMode
-  ForceMode.force 

Case

# ForceMode.force

A constant force or torque applied to a body, influencing motion over time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case force
```

## Discussion

The quantity that user sets via setForce(_:index:) has the units of mass \* distance / time^2. i.e. a force ( mass \* acceleration ). `force` mode causes a change in acceleration that varies proportionally to a body’s mass.

The quantity that user sets via setTorque(_:index:) has the units of mass \* distance^2 / time^2. `force` mode causes a change in angular acceleration that varies proportionally to a body’s mass and inertia.

