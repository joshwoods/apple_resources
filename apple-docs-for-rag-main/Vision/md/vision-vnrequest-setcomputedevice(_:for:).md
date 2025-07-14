

- Vision
- VNRequest
-  setComputeDevice(\_:for:) 

Instance Method

# setComputeDevice(\_:for:)

Assigns a compute device for a compute stage.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@nonobjc
func setComputeDevice(
    _ computeDevice: MLComputeDevice?,
    for computeStage: VNComputeStage
)
```

## Parameters 

`computeDevice`  

The compute device to assign to the compute stage.

`computeStage`  

The compute stage.

## Discussion

If the parameter `computeDevice` is `nil`, the framework removes any explicit compute device assignment and allows the framework to select the device.

Configure any compute device for a given compute stage. When performing a request, the system makes a validity check. Call supportedComputeStageDevices to get valid compute devices for a request’s compute stages.

## See Also

### Configuring the Compute Device

func computeDevice(for: VNComputeStage) -> MLComputeDevice?

Returns the compute device for a compute stage.

var supportedComputeStageDevices: [VNComputeStage : [MLComputeDevice]]

The collection of compute devices per stage that a request supports.

