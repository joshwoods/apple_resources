

- Matter
- MTRBaseClusterWiFiNetworkDiagnostics
-  readAttributeBeaconRxCount(completionHandler:) Deprecated

Instance Method

# readAttributeBeaconRxCount(completionHandler:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func readAttributeBeaconRxCount(completionHandler: @escaping (NSNumber?, (any Error)?) -> Void)
```

``` source
func readAttributeBeaconRxCount() async throws -> NSNumber
```

Deprecated

Please use readAttributeBeaconRxCountWithCompletion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func readAttributeBeaconRxCount() async throws -> NSNumber
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

