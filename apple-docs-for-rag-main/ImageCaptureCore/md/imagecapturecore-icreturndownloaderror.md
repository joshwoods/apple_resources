

- ImageCaptureCore
-  ICReturnDownloadError 

Structure

# ICReturnDownloadError

A download error returned from ImageCaptureCore.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
struct ICReturnDownloadError
```

## Topics

### Error Domain

let ICErrorDomain: String

An error returned by the ImageCaptureCore framework.

### Error Codes

static var fileWritable: ICReturnDownloadError.Code

The destination file is not writable.

static var pathInvalid: ICReturnDownloadError.Code

The destination path is invalid.

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

struct ICReturnMetadataError

A metadata error returned from ImageCaptureCore.

struct ICReturnObjectError

An object error returned from ImageCaptureCore.

struct ICReturnPTPDeviceError

A PTP device error returned from ImageCaptureCore.

struct ICReturnThumbnailError

A thumbnail error returned from ImageCaptureCore.

