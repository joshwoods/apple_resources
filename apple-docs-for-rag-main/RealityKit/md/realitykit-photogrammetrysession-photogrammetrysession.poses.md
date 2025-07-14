

- RealityKit
- PhotogrammetrySession
-  PhotogrammetrySession.Poses 

Structure

# PhotogrammetrySession.Poses

Once initial photogrammetric calculations are complete, a data structure mapping the sample ID (or index if a folder was used) to the 6DOF algorithmically estimated pose of that sample is returned.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct Poses
```

## Topics

### Instance Properties

let posesBySample: [Int : PhotogrammetrySession.Pose]

Mapping from the sample ID to the 6DOF algorithmically estimated pose of that sample. Each `Pose` will have a world translation and rotation representing that shot’s estimated pose (position and orientation in space) with respect to the estimated coordinate system.

var urlsBySample: [Int : URL]

Mapping from the sample ID to the image URL in the input folder corresponding to that sample ID. This simplifies the visualization of which image in the input folder corresponds to a given computed pose.

## See Also

### Obtaining results

enum Result

An object that holds the created 3D object.

struct PointCloud

A sparse point cloud data structure output as the payload of a `.pointCloud` request. A point cloud is an array of `PointCloud.Point` instances.

enum Error

The errors that can occur during reconstruction in a photogrammetry session.

struct Pose

A 6DOF pose relative to the estimated coordinate system.

