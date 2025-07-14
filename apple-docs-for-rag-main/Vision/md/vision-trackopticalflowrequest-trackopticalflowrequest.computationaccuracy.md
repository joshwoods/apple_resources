

- Vision
- TrackOpticalFlowRequest
-  TrackOpticalFlowRequest.ComputationAccuracy 

Enumeration

# TrackOpticalFlowRequest.ComputationAccuracy

A type that describes the computational accuracy.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum ComputationAccuracy
```

## Topics

### Getting the accuracies

case high

case low

case medium

case veryHigh

## Relationships

### Conforms To

- CaseIterable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting a request

var computationAccuracy: TrackOpticalFlowRequest.ComputationAccuracy

The level of accuracy to compute the optical flow.

var outputPixelFormatType: OSType

The desired pixel format type of the observation.

var supportedOutputPixelFormatTypes: [OSType]

The collection of supported pixel format types.

