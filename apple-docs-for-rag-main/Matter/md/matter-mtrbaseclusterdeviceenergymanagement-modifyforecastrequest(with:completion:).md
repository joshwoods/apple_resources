

- Matter
- MTRBaseClusterDeviceEnergyManagement
-  modifyForecastRequest(with:completion:) 

Instance Method

# modifyForecastRequest(with:completion:)

Command ModifyForecastRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func modifyForecastRequest(
    with params: MTRDeviceEnergyManagementClusterModifyForecastRequestParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func modifyForecastRequest(with params: MTRDeviceEnergyManagementClusterModifyForecastRequestParams) async throws
```

## Discussion

Allows a client to modify a Forecast within the limits allowed by the ESA.

