

- RealityKit
- PhotogrammetrySession
-  PhotogrammetrySession.Error 

Enumeration

# PhotogrammetrySession.Error

The errors that can occur during reconstruction in a photogrammetry session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
enum Error
```

## Overview

Localize these errors in your app.

## Topics

### Enumeration Cases

case insufficientStorage(requiredBytes: Int64)

An error that indicates insufficient storage space.

case invalidImages(URL)

An error that represents a problem with the image directory URL.

case invalidOutput(URL)

An error that represents an invalid output location.

### Instance Properties

var localizedDescription: String

Retrieve the localized description for this error.

### Default Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Error
- LocalizedError
- Sendable

## See Also

### Obtaining results

enum Result

An object that holds the created 3D object.

struct PointCloud

A sparse point cloud data structure output as the payload of a `.pointCloud` request. A point cloud is an array of `PointCloud.Point` instances.

struct Pose

A 6DOF pose relative to the estimated coordinate system.

struct Poses

Once initial photogrammetric calculations are complete, a data structure mapping the sample ID (or index if a folder was used) to the 6DOF algorithmically estimated pose of that sample is returned.

