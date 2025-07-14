

- Vision
- VNGenerateOpticalFlowRequest
-  outputPixelFormat 

Instance Property

# outputPixelFormat

The output buffer’s pixel format.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var outputPixelFormat: OSType { get set }
```

## See Also

### Configuring the Request

var computationAccuracy: VNGenerateOpticalFlowRequest.ComputationAccuracy

The accuracy level for computing optical flow.

enum ComputationAccuracy

The supported optical flow accuracy levels.

var keepNetworkOutput: Bool

A Boolean value that indicates whether to keep the raw pixel buffer coming from the machine learning network.

