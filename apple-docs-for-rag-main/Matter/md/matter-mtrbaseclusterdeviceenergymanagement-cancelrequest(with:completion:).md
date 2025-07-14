

- Matter
- MTRBaseClusterDeviceEnergyManagement
-  cancelRequest(with:completion:) 

Instance Method

# cancelRequest(with:completion:)

Command CancelRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func cancelRequest(
    with params: MTRDeviceEnergyManagementClusterCancelRequestParams?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func cancelRequest(with params: MTRDeviceEnergyManagementClusterCancelRequestParams?) async throws
```

## Discussion

Allows a client to request cancellation of a previous adjustment request in a StartTimeAdjustRequest, ModifyForecastRequest or RequestConstraintBasedForecast command.

