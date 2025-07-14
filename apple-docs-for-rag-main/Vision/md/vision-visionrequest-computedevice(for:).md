

- Vision
- VisionRequest
-  computeDevice(for:) 

Instance Method

# computeDevice(for:)

Returns the compute device for a compute stage.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func computeDevice(for computeStage: ComputeStage) -> MLComputeDevice?
```

**Required**

## Parameters 

`computeStage`  

The compute stage to inspect.

## Return Value

The current compute device; otherwise, `nil` if one isn’t assigned.

## See Also

### Getting the compute device

var supportedComputeStageDevices: [ComputeStage : [MLComputeDevice]]

The collection of compute devices per stage that a request supports.

**Required**

enum ComputeStage

Types that represent the compute stage.

