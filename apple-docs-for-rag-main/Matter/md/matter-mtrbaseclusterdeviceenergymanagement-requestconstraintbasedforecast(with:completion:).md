

- Matter
- MTRBaseClusterDeviceEnergyManagement
-  requestConstraintBasedForecast(with:completion:) 

Instance Method

# requestConstraintBasedForecast(with:completion:)

Command RequestConstraintBasedForecast

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func requestConstraintBasedForecast(
    with params: MTRDeviceEnergyManagementClusterRequestConstraintBasedForecastParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func requestConstraintBasedForecast(with params: MTRDeviceEnergyManagementClusterRequestConstraintBasedForecastParams) async throws
```

## Discussion

Allows a client to ask the ESA to recompute its Forecast based on power and time constraints.

