

- Vision
- TrackOpticalFlowRequest
-  computationAccuracy 

Instance Property

# computationAccuracy

The level of accuracy to compute the optical flow.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final var computationAccuracy: TrackOpticalFlowRequest.ComputationAccuracy { get set }
```

## Discussion

The computational time trends with accuracy level. The default value is TrackOpticalFlowRequest.ComputationAccuracy.high.

## See Also

### Inspecting a request

enum ComputationAccuracy

A type that describes the computational accuracy.

var outputPixelFormatType: OSType

The desired pixel format type of the observation.

var supportedOutputPixelFormatTypes: [OSType]

The collection of supported pixel format types.

