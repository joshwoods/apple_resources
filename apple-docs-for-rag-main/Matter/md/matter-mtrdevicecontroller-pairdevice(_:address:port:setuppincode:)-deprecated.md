

- Matter
- MTRDeviceController
-  pairDevice(\_:address:port:setupPINCode:) Deprecated

Instance Method

# pairDevice(\_:address:port:setupPINCode:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func pairDevice(
    _ deviceID: UInt64,
    address: String,
    port: UInt16,
    setupPINCode: UInt32
) throws
```

Deprecated

Please use setupCommissioningSessionWithPayload:newNodeID:error:

