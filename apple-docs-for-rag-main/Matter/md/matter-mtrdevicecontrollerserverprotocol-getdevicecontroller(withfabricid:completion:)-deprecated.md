

- Matter
- MTRDeviceControllerServerProtocol
-  getDeviceController(withFabricId:completion:) Deprecated

Instance Method

# getDeviceController(withFabricId:completion:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
optional func getDeviceController(
    withFabricId fabricId: UInt64,
    completion: @escaping MTRDeviceControllerGetterHandler
)
```

``` source
optional func deviceController(withFabricId fabricId: UInt64) async throws -> Any
```

Deprecated

This never called.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func deviceController(withFabricId fabricId: UInt64) async throws -> Any
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

