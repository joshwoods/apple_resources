

- Core Bluetooth
-  CBError 

Structure

# CBError

An error that Core Bluetooth returns during Bluetooth transactions.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CBError
```

## Topics

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

static var unkownDevice: CBError.Code

A misspelled version of the unknown device error code.

Deprecated

### Type Properties

static var encryptionTimedOut: CBError.Code

static var leGattExceededBackgroundNotificationLimit: CBError.Code

static var leGattNearBackgroundNotificationLimit: CBError.Code

static var peerRemovedPairingInformation: CBError.Code

static var tooManyLEPairedDevices: CBError.Code

static var errorDomain: String

### Enumerations

enum Code

The codes for errors that Core Bluetooth returns during Bluetooth transactions.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

let CBErrorDomain: String

The domain for Core Bluetooth errors.

enum Code

The codes for errors that Core Bluetooth returns during Bluetooth transactions.

struct CBATTError

An error that Core Bluetooth returns while using Attribute Protocol (ATT).

let CBATTErrorDomain: String

The domain for Core Bluetooth ATT errors.

enum Code

The possible errors returned by a GATT server (a remote peripheral) during Bluetooth low energy ATT transactions.

struct CBATTError

An error that Core Bluetooth returns while using Attribute Protocol (ATT).

