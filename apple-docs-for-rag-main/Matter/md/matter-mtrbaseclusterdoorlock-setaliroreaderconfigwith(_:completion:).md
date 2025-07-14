

- Matter
- MTRBaseClusterDoorLock
-  setAliroReaderConfigWith(\_:completion:) 

Instance Method

# setAliroReaderConfigWith(\_:completion:)

Command SetAliroReaderConfig

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func setAliroReaderConfigWith(
    _ params: MTRDoorLockClusterSetAliroReaderConfigParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func setAliroReaderConfigWith(_ params: MTRDoorLockClusterSetAliroReaderConfigParams) async throws
```

## Discussion

This command communicates an Aliro Reader configuration to the lock.

