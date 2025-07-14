

- Core Bluetooth
- CBError
-  unknownDevice 

Type Property

# unknownDevice

The device is unknown.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
static var unknownDevice: CBError.Code { get }
```

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

static var unkownDevice: CBError.Code

A misspelled version of the unknown device error code.

Deprecated

