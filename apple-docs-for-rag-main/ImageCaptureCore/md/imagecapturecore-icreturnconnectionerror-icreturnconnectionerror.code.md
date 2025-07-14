

- ImageCaptureCore
- ICReturnConnectionError
-  ICReturnConnectionError.Code 

Enumeration

# ICReturnConnectionError.Code

iOSiPadOSMac CatalystmacOSvisionOS

``` source
enum Code
```

## Topics

### Error Cases

case closedSessionSuddenly

Device closed session without request.

case driverExited

Device driver exited without request.

case ejectedSuddenly

Device ejected without request.

case ejectFailed

Device reports eject has failed.

case failedToOpen

Failed to open a connection to the device.

case failedToOpenDevice

Failed to open the device.

case sessionAlreadyOpen

Device reports session is already open.

case closedSessionSuddenly

Device closed session without request.

case driverExited

Device driver exited without request.

case ejectedSuddenly

Device ejected without request.

case ejectFailed

Device reports eject has failed.

case failedToOpen

Failed to open a connection to the device.

case failedToOpenDevice

Failed to open the device.

case sessionAlreadyOpen

Device reports session is already open.

### Enumeration Cases

case notAuthorizedToOpenDevice

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

### Error Codes

static var closedSessionSuddenly: ICReturnConnectionError.Code

Device closed session without request.

static var driverExited: ICReturnConnectionError.Code

Device driver exited without request.

static var ejectFailed: ICReturnConnectionError.Code

Device reports eject has failed.

static var ejectedSuddenly: ICReturnConnectionError.Code

Device ejected without request.

static var failedToOpen: ICReturnConnectionError.Code

Failed to open a connection to the device.

static var failedToOpenDevice: ICReturnConnectionError.Code

Failed to open the device.

static var sessionAlreadyOpen: ICReturnConnectionError.Code

Device reports session is already open.

