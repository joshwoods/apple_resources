

- Matter
- MTRBaseClusterDoorLock
-  unlockWithTimeout(with:completion:) 

Instance Method

# unlockWithTimeout(with:completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func unlockWithTimeout(
    with params: MTRDoorLockClusterUnlockWithTimeoutParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func unlockWithTimeout(with params: MTRDoorLockClusterUnlockWithTimeoutParams) async throws
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func unlockWithTimeout(with params: MTRDoorLockClusterUnlockWithTimeoutParams) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

