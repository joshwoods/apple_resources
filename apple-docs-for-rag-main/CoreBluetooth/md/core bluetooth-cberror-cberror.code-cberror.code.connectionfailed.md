

- Core Bluetooth
- CBError
- CBError.Code
-  CBError.Code.connectionFailed 

Case

# CBError.Code.connectionFailed

The connection failed.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.13+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case connectionFailed
```

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

case connectionLimitReached

The device already has the maximum number of connections.

case operationNotSupported

The operation isn’t supported.

static var unknownDevice: CBError.Code

The device is unknown.

case unkownDevice

A misspelled version of the unknown device error code.

Deprecated

