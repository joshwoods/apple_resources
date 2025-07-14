

- RealityKit
- PhotogrammetrySession
-  PhotogrammetrySession.PointCloud 

Structure

# PhotogrammetrySession.PointCloud

A sparse point cloud data structure output as the payload of a `.pointCloud` request. A point cloud is an array of `PointCloud.Point` instances.

iOS 17.0+iPadOS 17.0+Mac Catalyst 16.0+macOS 13.0+

``` source
struct PointCloud
```

## Topics

### Structures

struct Point

### Instance Properties

let points: [PhotogrammetrySession.PointCloud.Point]

The fixed array of points describing the point cloud.

## See Also

### Obtaining results

enum Result

An object that holds the created 3D object.

enum Error

The errors that can occur during reconstruction in a photogrammetry session.

struct Pose

A 6DOF pose relative to the estimated coordinate system.

struct Poses

Once initial photogrammetric calculations are complete, a data structure mapping the sample ID (or index if a folder was used) to the 6DOF algorithmically estimated pose of that sample is returned.

