

- Matter
- MTRBaseClusterTimeSynchronization
-  setTrustedTimeSourceWith(\_:completion:) 

Instance Method

# setTrustedTimeSourceWith(\_:completion:)

Command SetTrustedTimeSource

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func setTrustedTimeSourceWith(
    _ params: MTRTimeSynchronizationClusterSetTrustedTimeSourceParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func setTrustedTimeSourceWith(_ params: MTRTimeSynchronizationClusterSetTrustedTimeSourceParams) async throws
```

## Discussion

This command SHALL set TrustedTimeSource.

