

- Vision
- VNRequest
-  computeDevice(for:) 

Instance Method

# computeDevice(for:)

Returns the compute device for a compute stage.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@nonobjc
func computeDevice(for computeStage: VNComputeStage) -> MLComputeDevice?
```

## Parameters 

`computeStage`  

The compute stage to inspect.

## Return Value

The current compute device; otherwise, `nil` if one isn’t assigned.

## See Also

### Configuring the Compute Device

func setComputeDevice(MLComputeDevice?, for: VNComputeStage)

Assigns a compute device for a compute stage.

var supportedComputeStageDevices: [VNComputeStage : [MLComputeDevice]]

The collection of compute devices per stage that a request supports.

