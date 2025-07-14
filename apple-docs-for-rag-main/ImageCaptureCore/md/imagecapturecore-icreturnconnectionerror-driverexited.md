

- ImageCaptureCore
- ICReturnConnectionError
-  driverExited 

Type Property

# driverExited

Device driver exited without request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.9+visionOS 1.0+Xcode 11.0+

``` source
static var driverExited: ICReturnConnectionError.Code { get }
```

## See Also

### Error Codes

static var closedSessionSuddenly: ICReturnConnectionError.Code

Device closed session without request.

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

enum ICReturnConnectionError.Code

