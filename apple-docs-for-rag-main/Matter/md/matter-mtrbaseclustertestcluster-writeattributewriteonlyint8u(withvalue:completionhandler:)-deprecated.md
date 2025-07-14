

- Matter
- MTRBaseClusterTestCluster
-  writeAttributeWriteOnlyInt8u(withValue:completionHandler:) Deprecated

Instance Method

# writeAttributeWriteOnlyInt8u(withValue:completionHandler:)

iOS 16.2–16.4DeprecatediPadOS 16.2–16.4DeprecatedMac Catalyst 16.2–16.4DeprecatedmacOS 13.1–13.3DeprecatedtvOS 16.2–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.2–9.4Deprecated

``` source
func writeAttributeWriteOnlyInt8u(
    withValue value: NSNumber,
    completionHandler: @escaping MTRStatusCompletion
)
```

``` source
func writeAttributeWriteOnlyInt8u(withValue value: NSNumber) async throws
```

Deprecated

Please use writeAttributeWriteOnlyInt8uWithValue:completion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func writeAttributeWriteOnlyInt8u(withValue value: NSNumber) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

