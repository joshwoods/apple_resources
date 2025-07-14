

- Matter
- MTRBaseClusterTimeSynchronization
-  setUTCTimeWith(\_:completion:) 

Instance Method

# setUTCTimeWith(\_:completion:)

Command SetUTCTime

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func setUTCTimeWith(
    _ params: MTRTimeSynchronizationClusterSetUTCTimeParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func setUTCTimeWith(_ params: MTRTimeSynchronizationClusterSetUTCTimeParams) async throws
```

## Discussion

This command MAY be issued by Administrator to set the time.

