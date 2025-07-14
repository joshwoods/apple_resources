

- Core Bluetooth
- CBError
- CBError.Code
-  CBError.Code.unkownDevice Deprecated

Case

# CBError.Code.unkownDevice

A misspelled version of the unknown device error code.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.13–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
case unkownDevice
```

Deprecated

Use unknownDevice instead.

## See Also

### Error Codes

case unknown

An unknown error occurred.

case invalidParameters

The specified parameters are invalid.

case invalidHandle

The specified attribute handle is invalid.

case notConnected

The device isn’t currently connected.

case outOfSpace

The device has run out of space to complete the intended operation.

case operationCancelled

The error represents a canceled operation.

case connectionTimeout

The connection timed out.

case peripheralDisconnected

The peripheral disconnected.

case uuidNotAllowed

The specified UUID isn’t permitted.

case alreadyAdvertising

The peripheral is already advertising.

case connectionFailed

The connection failed.

case connectionLimitReached

The device already has the maximum number of connections.

case operationNotSupported

The operation isn’t supported.

static var unknownDevice: CBError.Code

The device is unknown.

