

- Vision
- VNTrackOpticalFlowRequest
-  outputPixelFormat 

Instance Property

# outputPixelFormat

The pixel format type of the output value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var outputPixelFormat: OSType { get set }
```

## Discussion

The valid values are kCVPixelFormatType_TwoComponent32Float and kCVPixelFormatType_TwoComponent16Half. The default value is kCVPixelFormatType_TwoComponent32Float.

## See Also

### Configuring the Request

var computationAccuracy: VNTrackOpticalFlowRequest.ComputationAccuracy

The level of accuracy to compute the optical flow.

enum ComputationAccuracy

Computational accuracy options.

var keepNetworkOutput: Bool

A Boolean value that indicates the raw pixel buffer continues to emit from the network.

