

- RealityKit
- PhotogrammetrySession
-  PhotogrammetrySession.Result 

Enumeration

# PhotogrammetrySession.Result

An object that holds the created 3D object.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum Result
```

## Overview

When PhotogrammetrySession completes a PhotogrammetrySession.Request, it publishes a PhotogrammetrySession.Output.requestComplete(_:_:) message to output, and includes the created object as the associated value of the result parameter. The result type corresponds to the request type. For example, a PhotogrammetrySession.Request.modelFile(url:detail:geometry:) request results in the session publishing a PhotogrammetrySession.Result.modelFile(_:).

## Topics

### Types of output

case modelFile(URL)

The result of a request for a USDZ file.

case modelEntity(ModelEntity)

The result of a request for an in-memory entity.

case bounds(BoundingBox)

The result of a request for a bounding box.

### Enumeration Cases

case pointCloud(PhotogrammetrySession.PointCloud)

The result of a request for a point cloud.

case poses(PhotogrammetrySession.Poses)

Once initial photogrammetric calculations are complete, a data structure mapping each sample ID (or index if a folder was used) to the 6DOF algorithmically estimated pose of that sample is returned.

## See Also

### Obtaining results

struct PointCloud

A sparse point cloud data structure output as the payload of a `.pointCloud` request. A point cloud is an array of `PointCloud.Point` instances.

enum Error

The errors that can occur during reconstruction in a photogrammetry session.

struct Pose

A 6DOF pose relative to the estimated coordinate system.

struct Poses

Once initial photogrammetric calculations are complete, a data structure mapping the sample ID (or index if a folder was used) to the 6DOF algorithmically estimated pose of that sample is returned.

