

- Matter
- MTRBaseClusterICDManagement
-  unregisterClient(with:completion:) 

Instance Method

# unregisterClient(with:completion:)

Command UnregisterClient

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func unregisterClient(
    with params: MTRICDManagementClusterUnregisterClientParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func unregisterClient(with params: MTRICDManagementClusterUnregisterClientParams) async throws
```

## Discussion

Unregister a client from an end device

