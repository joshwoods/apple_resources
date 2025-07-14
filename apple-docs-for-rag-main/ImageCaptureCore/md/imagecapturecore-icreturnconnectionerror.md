

- ImageCaptureCore
-  ICReturnConnectionError 

Structure

# ICReturnConnectionError

A connection error returned from ImageCaptureCore.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
struct ICReturnConnectionError
```

## Topics

### Error Domain

let ICErrorDomain: String

An error returned by the ImageCaptureCore framework.

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

enum Code

### Type Properties

static var errorDomain: String

static var notAuthorizedToOpenDevice: ICReturnConnectionError.Code

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

ICReturn

An error returned from ImageCaptureCore.

ICLegacyReturn

A legacy error returned from ImageCaptureCore.

struct ICReturnDownloadError

A download error returned from ImageCaptureCore.

struct ICReturnMetadataError

A metadata error returned from ImageCaptureCore.

struct ICReturnObjectError

An object error returned from ImageCaptureCore.

struct ICReturnPTPDeviceError

A PTP device error returned from ImageCaptureCore.

struct ICReturnThumbnailError

A thumbnail error returned from ImageCaptureCore.

