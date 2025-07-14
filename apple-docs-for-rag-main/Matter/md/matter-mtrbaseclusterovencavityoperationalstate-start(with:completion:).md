

- Matter
- MTRBaseClusterOvenCavityOperationalState
-  start(with:completion:) 

Instance Method

# start(with:completion:)

Command Start

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func start(
    with params: MTROvenCavityOperationalStateClusterStartParams?,
    completion: @escaping (MTROvenCavityOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void
)
```

``` source
func start(with params: MTROvenCavityOperationalStateClusterStartParams?) async throws -> MTROvenCavityOperationalStateClusterOperationalCommandResponseParams
```

## Discussion

Upon receipt, the device SHALL start its operation if it is safe to do so and the device is in an operational state from which it can be started.

