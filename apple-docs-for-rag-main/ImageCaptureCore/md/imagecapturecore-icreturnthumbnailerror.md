

- ImageCaptureCore
-  ICReturnThumbnailError 

Structure

# ICReturnThumbnailError

A thumbnail error returned from ImageCaptureCore.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
struct ICReturnThumbnailError
```

## Topics

### Error Domain

let ICErrorDomain: String

An error returned by the ImageCaptureCore framework.

### Error Codes

static var alreadyFetching: ICReturnThumbnailError.Code

Item thumbnail request is being serviced.

static var canceled: ICReturnThumbnailError.Code

Item thumbnail request has been canceled.

static var invalid: ICReturnThumbnailError.Code

Item thumbnail request completed with invalid result.

static var notAvailable: ICReturnThumbnailError.Code

Item does not have thumbnail available.

enum Code

### Type Properties

static var errorDomain: String

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

struct ICReturnConnectionError

A connection error returned from ImageCaptureCore.

struct ICReturnDownloadError

A download error returned from ImageCaptureCore.

struct ICReturnMetadataError

A metadata error returned from ImageCaptureCore.

struct ICReturnObjectError

An object error returned from ImageCaptureCore.

struct ICReturnPTPDeviceError

A PTP device error returned from ImageCaptureCore.

