

- Vision
- VNRequest
-  supportedComputeStageDevices 

Instance Property

# supportedComputeStageDevices

The collection of compute devices per stage that a request supports.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@nonobjc
var supportedComputeStageDevices: [VNComputeStage : [MLComputeDevice]] { get throws }
```

## Discussion

A dictionary of per-stage compute devices; otherwise, `nil` if an error occurs.

## See Also

### Configuring the Compute Device

func setComputeDevice(MLComputeDevice?, for: VNComputeStage)

Assigns a compute device for a compute stage.

func computeDevice(for: VNComputeStage) -> MLComputeDevice?

Returns the compute device for a compute stage.

