

- Core Bluetooth
- CBError
-  CBError.Code 

Enumeration

# CBError.Code

The codes for errors that Core Bluetooth returns during Bluetooth transactions.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
enum Code
```

## Topics

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

case unkownDevice

A misspelled version of the unknown device error code.

Deprecated

### Enumeration Cases

case encryptionTimedOut

case leGattExceededBackgroundNotificationLimit

case leGattNearBackgroundNotificationLimit

case peerRemovedPairingInformation

case tooManyLEPairedDevices

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct CBError

An error that Core Bluetooth returns during Bluetooth transactions.

let CBErrorDomain: String

The domain for Core Bluetooth errors.

struct CBATTError

An error that Core Bluetooth returns while using Attribute Protocol (ATT).

let CBATTErrorDomain: String

The domain for Core Bluetooth ATT errors.

enum Code

The possible errors returned by a GATT server (a remote peripheral) during Bluetooth low energy ATT transactions.

struct CBATTError

An error that Core Bluetooth returns while using Attribute Protocol (ATT).

