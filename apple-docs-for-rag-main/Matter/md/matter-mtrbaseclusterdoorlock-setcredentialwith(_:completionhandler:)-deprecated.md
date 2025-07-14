

- Matter
- MTRBaseClusterDoorLock
-  setCredentialWith(\_:completionHandler:) Deprecated

Instance Method

# setCredentialWith(\_:completionHandler:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func setCredentialWith(
    _ params: MTRDoorLockClusterSetCredentialParams,
    completionHandler: @escaping (MTRDoorLockClusterSetCredentialResponseParams?, (any Error)?) -> Void
)
```

``` source
func setCredentialWith(_ params: MTRDoorLockClusterSetCredentialParams) async throws -> MTRDoorLockClusterSetCredentialResponseParams
```

Deprecated

Please use setCredentialWithParams:completion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setCredentialWith(_ params: MTRDoorLockClusterSetCredentialParams) async throws -> MTRDoorLockClusterSetCredentialResponseParams
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

