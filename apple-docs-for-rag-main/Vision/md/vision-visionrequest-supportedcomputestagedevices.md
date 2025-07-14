

- Vision
- VisionRequest
-  supportedComputeStageDevices 

Instance Property

# supportedComputeStageDevices

The collection of compute devices per stage that a request supports.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var supportedComputeStageDevices: [ComputeStage : [MLComputeDevice]] { get }
```

**Required**

## See Also

### Getting the compute device

func computeDevice(for: ComputeStage) -> MLComputeDevice?

Returns the compute device for a compute stage.

**Required**

enum ComputeStage

Types that represent the compute stage.

