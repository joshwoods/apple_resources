

- Matter
- MTRBaseClusterTimeSynchronization
-  setDSTOffsetWith(\_:completion:) 

Instance Method

# setDSTOffsetWith(\_:completion:)

Command SetDSTOffset

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func setDSTOffsetWith(
    _ params: MTRTimeSynchronizationClusterSetDSTOffsetParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func setDSTOffsetWith(_ params: MTRTimeSynchronizationClusterSetDSTOffsetParams) async throws
```

## Discussion

This command SHALL set DSTOffset.

