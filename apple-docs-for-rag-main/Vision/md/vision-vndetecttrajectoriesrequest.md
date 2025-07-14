

- Vision
-  VNDetectTrajectoriesRequest 

Class

# VNDetectTrajectoriesRequest

A request that detects the trajectories of shapes moving along a parabolic path.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNDetectTrajectoriesRequest
```

## Mentioned in 

Identifying Trajectories in Video

## Overview

After the request detects a trajectory, it produces an observation that contains the shape’s detected points and an equation describing the parabola.

## Topics

### Creating a Request

init(frameAnalysisSpacing: CMTime, trajectoryLength: Int, completionHandler: VNRequestCompletionHandler?)

Creates a new request to detect trajectories.

### Configuring the Request

var targetFrameTime: CMTime

The requested target frame time for processing trajectory detection.

var trajectoryLength: Int

The number of points to detect before calculating a trajectory.

var objectMinimumNormalizedRadius: Float

The minimum radius of the bounding circle of the object to track.

var objectMaximumNormalizedRadius: Float

The maximum radius of the bounding circle of the object to track.

var minimumObjectSize: Float

The minimum radius of the tracked shape’s bounding circle.

Deprecated

var maximumObjectSize: Float

The maximum radius of the tracked shape’s bounding circle.

Deprecated

### Inspecting the Results

var results: [VNTrajectoryObservation]?

The array of detected trajectory observations.

class VNTrajectoryObservation

An observation that describes a detected trajectory.

### Identifying Request Revisions

let VNDetectTrajectoriesRequestRevision1: Int

A constant for specifying revision 1 of the trajectories detection request.

## Relationships

### Inherits From

- VNStatefulRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Trajectory detection

Identifying Trajectories in Video

Gain new insights into your video data by using Vision to detect trajectories.

Detecting moving objects in a video

Identify the trajectory of a thrown object by using Vision.

