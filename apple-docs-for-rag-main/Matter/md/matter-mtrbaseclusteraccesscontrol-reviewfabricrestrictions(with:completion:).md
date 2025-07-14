

- Matter
- MTRBaseClusterAccessControl
-  reviewFabricRestrictions(with:completion:) 

Instance Method

# reviewFabricRestrictions(with:completion:)

Command ReviewFabricRestrictions

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func reviewFabricRestrictions(
    with params: MTRAccessControlClusterReviewFabricRestrictionsParams,
    completion: @escaping (MTRAccessControlClusterReviewFabricRestrictionsResponseParams?, (any Error)?) -> Void
)
```

``` source
func reviewFabricRestrictions(with params: MTRAccessControlClusterReviewFabricRestrictionsParams) async throws -> MTRAccessControlClusterReviewFabricRestrictionsResponseParams
```

## Discussion

This command signals to the service associated with the device vendor that the fabric administrator would like a review of the current restrictions on the accessing fabric.

