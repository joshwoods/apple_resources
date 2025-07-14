

- Matter
- MTRBaseClusterThreadNetworkDirectory
-  getOperationalDataset(with:completion:) 

Instance Method

# getOperationalDataset(with:completion:)

Command GetOperationalDataset

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func getOperationalDataset(
    with params: MTRThreadNetworkDirectoryClusterGetOperationalDatasetParams,
    completion: @escaping (MTRThreadNetworkDirectoryClusterOperationalDatasetResponseParams?, (any Error)?) -> Void
)
```

``` source
func operationalDataset(with params: MTRThreadNetworkDirectoryClusterGetOperationalDatasetParams) async throws -> MTRThreadNetworkDirectoryClusterOperationalDatasetResponseParams
```

## Discussion

Retrieves a Thread Operational Dataset from the ThreadNetworks list.

