

- Matter
- MTRBaseClusterDeviceEnergyManagement
-  powerAdjustRequest(with:completion:) 

Instance Method

# powerAdjustRequest(with:completion:)

Command PowerAdjustRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func powerAdjustRequest(
    with params: MTRDeviceEnergyManagementClusterPowerAdjustRequestParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func powerAdjustRequest(with params: MTRDeviceEnergyManagementClusterPowerAdjustRequestParams) async throws
```

## Discussion

Allows a client to request an adjustment in the power consumption of an ESA for a specified duration.

