

- Matter
- MTRBaseClusterDoorLock
-  clearAliroReaderConfig(with:completion:) 

Instance Method

# clearAliroReaderConfig(with:completion:)

Command ClearAliroReaderConfig

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func clearAliroReaderConfig(
    with params: MTRDoorLockClusterClearAliroReaderConfigParams?,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func clearAliroReaderConfig(with params: MTRDoorLockClusterClearAliroReaderConfigParams?) async throws
```

## Discussion

This command clears an existing Aliro Reader configuration for the lock.

