

- Vision
- TrackOpticalFlowRequest
-  outputPixelFormatType 

Instance Property

# outputPixelFormatType

The desired pixel format type of the observation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final var outputPixelFormatType: OSType { get set }
```

## Discussion

The default is kCVPixelFormatType_TwoComponent32Float.

## See Also

### Inspecting a request

var computationAccuracy: TrackOpticalFlowRequest.ComputationAccuracy

The level of accuracy to compute the optical flow.

enum ComputationAccuracy

A type that describes the computational accuracy.

var supportedOutputPixelFormatTypes: [OSType]

The collection of supported pixel format types.

