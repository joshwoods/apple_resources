

- Core Bluetooth
- CBError
-  unkownDevice Deprecated

Type Property

# unkownDevice

A misspelled version of the unknown device error code.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.13–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
static var unkownDevice: CBError.Code { get }
```

Deprecated

Use unknownDevice instead.

## See Also

### Error Codes

static var unknown: CBError.Code

An unknown error occurred.

static var invalidParameters: CBError.Code

The specified parameters are invalid.

static var invalidHandle: CBError.Code

The specified attribute handle is invalid.

static var notConnected: CBError.Code

The device isn’t currently connected.

static var outOfSpace: CBError.Code

The device has run out of space to complete the intended operation.

static var operationCancelled: CBError.Code

The error represents a canceled operation.

static var connectionTimeout: CBError.Code

The connection timed out.

static var peripheralDisconnected: CBError.Code

The peripheral disconnected.

static var uuidNotAllowed: CBError.Code

The specified UUID isn’t permitted.

static var alreadyAdvertising: CBError.Code

The peripheral is already advertising.

static var connectionFailed: CBError.Code

The connection failed.

static var connectionLimitReached: CBError.Code

The device already has the maximum number of connections.

static var operationNotSupported: CBError.Code

The operation isn’t supported.

static var unknownDevice: CBError.Code

The device is unknown.

