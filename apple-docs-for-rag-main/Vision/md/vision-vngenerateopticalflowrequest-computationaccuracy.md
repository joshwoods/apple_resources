

- Vision
- VNGenerateOpticalFlowRequest
-  computationAccuracy 

Instance Property

# computationAccuracy

The accuracy level for computing optical flow.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var computationAccuracy: VNGenerateOpticalFlowRequest.ComputationAccuracy { get set }
```

## See Also

### Configuring the Request

enum ComputationAccuracy

The supported optical flow accuracy levels.

var outputPixelFormat: OSType

The output buffer’s pixel format.

var keepNetworkOutput: Bool

A Boolean value that indicates whether to keep the raw pixel buffer coming from the machine learning network.

