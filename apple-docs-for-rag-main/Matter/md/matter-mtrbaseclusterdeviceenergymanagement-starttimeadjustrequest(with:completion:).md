

- Matter
- MTRBaseClusterDeviceEnergyManagement
-  startTimeAdjustRequest(with:completion:) 

Instance Method

# startTimeAdjustRequest(with:completion:)

Command StartTimeAdjustRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func startTimeAdjustRequest(
    with params: MTRDeviceEnergyManagementClusterStartTimeAdjustRequestParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func startTimeAdjustRequest(with params: MTRDeviceEnergyManagementClusterStartTimeAdjustRequestParams) async throws
```

## Discussion

Allows a client to adjust the start time of a Forecast sequence that has not yet started operation (i.e. where the current Forecast StartTime is in the future).

