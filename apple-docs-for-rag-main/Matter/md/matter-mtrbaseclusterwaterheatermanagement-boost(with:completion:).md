

- Matter
- MTRBaseClusterWaterHeaterManagement
-  boost(with:completion:) 

Instance Method

# boost(with:completion:)

Command Boost

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func boost(
    with params: MTRWaterHeaterManagementClusterBoostParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func boost(with params: MTRWaterHeaterManagementClusterBoostParams) async throws
```

## Discussion

Allows a client to request that the water heater is put into a Boost state.

