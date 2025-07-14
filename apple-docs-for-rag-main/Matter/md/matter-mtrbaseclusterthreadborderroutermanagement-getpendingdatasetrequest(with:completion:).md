

- Matter
- MTRBaseClusterThreadBorderRouterManagement
-  getPendingDatasetRequest(with:completion:) 

Instance Method

# getPendingDatasetRequest(with:completion:)

Command GetPendingDatasetRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func getPendingDatasetRequest(
    with params: MTRThreadBorderRouterManagementClusterGetPendingDatasetRequestParams?,
    completion: @escaping (MTRThreadBorderRouterManagementClusterDatasetResponseParams?, (any Error)?) -> Void
)
```

``` source
func pendingDatasetRequest(with params: MTRThreadBorderRouterManagementClusterGetPendingDatasetRequestParams?) async throws -> MTRThreadBorderRouterManagementClusterDatasetResponseParams
```

## Discussion

Command to request the pending dataset of the Thread network to which the border router is connected. This command must be sent over a valid CASE session

