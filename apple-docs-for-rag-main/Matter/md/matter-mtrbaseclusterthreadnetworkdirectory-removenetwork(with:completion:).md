

- Matter
- MTRBaseClusterThreadNetworkDirectory
-  removeNetwork(with:completion:) 

Instance Method

# removeNetwork(with:completion:)

Command RemoveNetwork

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func removeNetwork(
    with params: MTRThreadNetworkDirectoryClusterRemoveNetworkParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func removeNetwork(with params: MTRThreadNetworkDirectoryClusterRemoveNetworkParams) async throws
```

## Discussion

Removes an entry from the ThreadNetworks list.

