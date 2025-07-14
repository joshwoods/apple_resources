

- RealityKit
- PhotogrammetrySession
-  PhotogrammetrySession.Pose 

Structure

# PhotogrammetrySession.Pose

A 6DOF pose relative to the estimated coordinate system.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct Pose
```

## Topics

### Instance Properties

let rotation: simd_quatf

Rotation (orientation) of the pose relative to the reference coordinate system.

var transform: Transform

A unit scale transform that represents a 6DoF pose.

let translation: SIMD3&lt;Float>

Position of the pose relative to the reference coordinate system.

## See Also

### Obtaining results

enum Result

An object that holds the created 3D object.

struct PointCloud

A sparse point cloud data structure output as the payload of a `.pointCloud` request. A point cloud is an array of `PointCloud.Point` instances.

enum Error

The errors that can occur during reconstruction in a photogrammetry session.

struct Poses

Once initial photogrammetric calculations are complete, a data structure mapping the sample ID (or index if a folder was used) to the 6DOF algorithmically estimated pose of that sample is returned.

