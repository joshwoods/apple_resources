

- Matter
- MTRBaseClusterThreadBorderRouterManagement
-  getActiveDatasetRequest(with:completion:) 

Instance Method

# getActiveDatasetRequest(with:completion:)

Command GetActiveDatasetRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func getActiveDatasetRequest(
    with params: MTRThreadBorderRouterManagementClusterGetActiveDatasetRequestParams?,
    completion: @escaping (MTRThreadBorderRouterManagementClusterDatasetResponseParams?, (any Error)?) -> Void
)
```

``` source
func activeDatasetRequest(with params: MTRThreadBorderRouterManagementClusterGetActiveDatasetRequestParams?) async throws -> MTRThreadBorderRouterManagementClusterDatasetResponseParams
```

## Discussion

Command to request the active operational dataset of the Thread network to which the border router is connected. This command must be sent over a valid CASE session

