

- Matter
- MTRBaseClusterServiceArea
-  skip(with:completion:) 

Instance Method

# skip(with:completion:)

Command SkipArea

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func skip(
    with params: MTRServiceAreaClusterSkipAreaParams,
    completion: @escaping (MTRServiceAreaClusterSkipAreaResponseParams?, (any Error)?) -> Void
)
```

``` source
func skip(with params: MTRServiceAreaClusterSkipAreaParams) async throws -> MTRServiceAreaClusterSkipAreaResponseParams
```

## Discussion

This command is used to skip an area where the device operates.

