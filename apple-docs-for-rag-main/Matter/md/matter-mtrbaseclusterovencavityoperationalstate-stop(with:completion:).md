

- Matter
- MTRBaseClusterOvenCavityOperationalState
-  stop(with:completion:) 

Instance Method

# stop(with:completion:)

Command Stop

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func stop(
    with params: MTROvenCavityOperationalStateClusterStopParams?,
    completion: @escaping (MTROvenCavityOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void
)
```

``` source
func stop(with params: MTROvenCavityOperationalStateClusterStopParams?) async throws -> MTROvenCavityOperationalStateClusterOperationalCommandResponseParams
```

## Discussion

Upon receipt, the device SHALL stop its operation if it is at a position where it is safe to do so and/or permitted.

