

- Matter
- MTRBaseClusterRVCOperationalState
-  goHome(with:completion:) 

Instance Method

# goHome(with:completion:)

Command GoHome

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func goHome(
    with params: MTRRVCOperationalStateClusterGoHomeParams?,
    completion: @escaping (MTRRVCOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void
)
```

``` source
func goHome(with params: MTRRVCOperationalStateClusterGoHomeParams?) async throws -> MTRRVCOperationalStateClusterOperationalCommandResponseParams
```

## Discussion

On receipt of this command, the device SHALL start seeking the charging dock, if possible in the current state of the device.

