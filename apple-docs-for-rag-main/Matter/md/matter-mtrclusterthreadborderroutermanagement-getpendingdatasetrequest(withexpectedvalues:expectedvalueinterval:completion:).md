

- Matter
- MTRClusterThreadBorderRouterManagement
-  getPendingDatasetRequest(withExpectedValues:expectedValueInterval:completion:) 

Instance Method

# getPendingDatasetRequest(withExpectedValues:expectedValueInterval:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func getPendingDatasetRequest(
    withExpectedValues expectedValues: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTRThreadBorderRouterManagementClusterDatasetResponseParams?, (any Error)?) -> Void
)
```

``` source
func pendingDatasetRequest(
    withExpectedValues expectedValues: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTRThreadBorderRouterManagementClusterDatasetResponseParams
```

