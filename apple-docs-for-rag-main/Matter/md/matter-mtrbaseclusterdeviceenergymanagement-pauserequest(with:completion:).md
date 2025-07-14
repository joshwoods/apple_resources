

- Matter
- MTRBaseClusterDeviceEnergyManagement
-  pauseRequest(with:completion:) 

Instance Method

# pauseRequest(with:completion:)

Command PauseRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func pauseRequest(
    with params: MTRDeviceEnergyManagementClusterPauseRequestParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func pauseRequest(with params: MTRDeviceEnergyManagementClusterPauseRequestParams) async throws
```

## Discussion

Allows a client to temporarily pause an operation and reduce the ESAs energy demand.

