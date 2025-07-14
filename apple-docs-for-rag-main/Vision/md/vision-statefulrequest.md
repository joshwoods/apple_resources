

- Vision
-  StatefulRequest 

Protocol

# StatefulRequest

The protocol for a type that builds evidence of a condition over time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
protocol StatefulRequest : VisionRequest
```

## Topics

### Inspecting the request

var frameAnalysisSpacing: CMTime

The reciprocal of the maximum rate to process buffers.

**Required**

var minimumLatencyFrameCount: Int

The minimum number of frames that the request has to process before reporting any observations.

**Required** Default implementation provided.

### Comparing the request

static func == (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Hashing the request

func hash(into: inout Hasher)

Hashes the essential components of the value by passing them into the hasher.

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Inherits From

- CustomStringConvertible
- Equatable
- Hashable
- Sendable
- VisionRequest

### Conforming Types

- DetectHumanBodyPose3DRequest
- DetectTrajectoriesRequest
- GeneratePersonSegmentationRequest
- TrackHomographicImageRegistrationRequest
- TrackObjectRequest
- TrackOpticalFlowRequest
- TrackRectangleRequest
- TrackTranslationalImageRegistrationRequest

## See Also

### Image sequence analysis

class GeneratePersonSegmentationRequest

A request that produces a matte image for a person it finds in the input image.

struct GeneratePersonInstanceMaskRequest

A request that produces a mask of individual people it finds in the input image.

struct DetectDocumentSegmentationRequest

A request that detects rectangular regions that contain text in the input image.

