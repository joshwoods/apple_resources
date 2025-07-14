

- Matter
- MTRDeviceController
-  getBaseDevice(\_:queue:completionHandler:) Deprecated

Instance Method

# getBaseDevice(\_:queue:completionHandler:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func getBaseDevice(
    _ deviceID: UInt64,
    queue: dispatch_queue_t,
    completionHandler: @escaping MTRDeviceConnectionCallback
) -> Bool
```

Deprecated

Please use \[MTRBaseDevice deviceWithNodeID:controller:\]

