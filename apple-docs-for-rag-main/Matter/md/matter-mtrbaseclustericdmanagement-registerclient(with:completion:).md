

- Matter
- MTRBaseClusterICDManagement
-  registerClient(with:completion:) 

Instance Method

# registerClient(with:completion:)

Command RegisterClient

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func registerClient(
    with params: MTRICDManagementClusterRegisterClientParams,
    completion: @escaping (MTRICDManagementClusterRegisterClientResponseParams?, (any Error)?) -> Void
)
```

``` source
func registerClient(with params: MTRICDManagementClusterRegisterClientParams) async throws -> MTRICDManagementClusterRegisterClientResponseParams
```

## Discussion

Register a client to the end device

