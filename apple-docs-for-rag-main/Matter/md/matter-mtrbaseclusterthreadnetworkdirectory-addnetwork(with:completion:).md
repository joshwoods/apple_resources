

- Matter
- MTRBaseClusterThreadNetworkDirectory
-  addNetwork(with:completion:) 

Instance Method

# addNetwork(with:completion:)

Command AddNetwork

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func addNetwork(
    with params: MTRThreadNetworkDirectoryClusterAddNetworkParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func addNetwork(with params: MTRThreadNetworkDirectoryClusterAddNetworkParams) async throws
```

## Discussion

Adds an entry to the ThreadNetworks list.

