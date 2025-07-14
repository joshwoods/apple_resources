

- Matter
- MTRBaseClusterWaterHeaterManagement
-  cancelBoost(with:completion:) 

Instance Method

# cancelBoost(with:completion:)

Command CancelBoost

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func cancelBoost(
    with params: MTRWaterHeaterManagementClusterCancelBoostParams?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func cancelBoost(with params: MTRWaterHeaterManagementClusterCancelBoostParams?) async throws
```

## Discussion

Allows a client to cancel an ongoing Boost operation.

