

- Matter
- MTRBaseClusterTimeSynchronization
-  setTimeZoneWith(\_:completion:) 

Instance Method

# setTimeZoneWith(\_:completion:)

Command SetTimeZone

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func setTimeZoneWith(
    _ params: MTRTimeSynchronizationClusterSetTimeZoneParams,
    completion: @escaping (MTRTimeSynchronizationClusterSetTimeZoneResponseParams?, (any Error)?) -> Void
)
```

``` source
func setTimeZoneWith(_ params: MTRTimeSynchronizationClusterSetTimeZoneParams) async throws -> MTRTimeSynchronizationClusterSetTimeZoneResponseParams
```

## Discussion

This command SHALL set TimeZone.

