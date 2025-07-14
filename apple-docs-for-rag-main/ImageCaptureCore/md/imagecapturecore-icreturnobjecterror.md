

- ImageCaptureCore
-  ICReturnObjectError 

Structure

# ICReturnObjectError

An object error returned from ImageCaptureCore.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
struct ICReturnObjectError
```

## Topics

### Error Domain

let ICErrorDomain: String

An error returned by the ImageCaptureCore framework.

### Error Codes

static var codeObjectDoesNotExist: ICReturnObjectError.Code

The object does not exist.

static var codeObjectDataOffsetInvalid: ICReturnObjectError.Code

The object data offset is invalid.

static var codeObjectCouldNotBeRead: ICReturnObjectError.Code

The object could not be read.

static var codeObjectDataEmpty: ICReturnObjectError.Code

The object data is empty.

enum Code

### Type Properties

static var codeObjectDataRequestTooLarge: ICReturnObjectError.Code

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

struct ICReturnPTPDeviceError

A PTP device error returned from ImageCaptureCore.

struct ICReturnThumbnailError

A thumbnail error returned from ImageCaptureCore.

