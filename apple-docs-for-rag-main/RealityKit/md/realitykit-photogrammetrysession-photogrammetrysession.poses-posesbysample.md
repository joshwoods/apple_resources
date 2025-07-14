

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Poses
-  posesBySample 

Instance Property

# posesBySample

Mapping from the sample ID to the 6DOF algorithmically estimated pose of that sample. Each `Pose` will have a world translation and rotation representing that shot’s estimated pose (position and orientation in space) with respect to the estimated coordinate system.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
let posesBySample: [Int : PhotogrammetrySession.Pose]
```

