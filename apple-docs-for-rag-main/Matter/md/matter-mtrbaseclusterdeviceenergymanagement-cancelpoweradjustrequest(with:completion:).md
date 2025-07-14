

- Matter
- MTRBaseClusterDeviceEnergyManagement
-  cancelPowerAdjustRequest(with:completion:) 

Instance Method

# cancelPowerAdjustRequest(with:completion:)

Command CancelPowerAdjustRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func cancelPowerAdjustRequest(
    with params: MTRDeviceEnergyManagementClusterCancelPowerAdjustRequestParams?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func cancelPowerAdjustRequest(with params: MTRDeviceEnergyManagementClusterCancelPowerAdjustRequestParams?) async throws
```

## Discussion

Allows a client to cancel an ongoing PowerAdjustmentRequest operation.

