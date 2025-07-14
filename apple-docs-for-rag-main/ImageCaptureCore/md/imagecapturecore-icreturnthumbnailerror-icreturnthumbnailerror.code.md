

- ImageCaptureCore
- ICReturnThumbnailError
-  ICReturnThumbnailError.Code 

Enumeration

# ICReturnThumbnailError.Code

iOSiPadOSMac CatalystmacOSvisionOS

``` source
enum Code
```

## Topics

### Error Cases

case alreadyFetching

Item thumbnail request is being serviced.

case canceled

Item thumbnail request has been canceled.

case invalid

Item thumbnail request completed with invalid result.

case notAvailable

Item does not have thumbnail available.

case alreadyFetching

Item thumbnail request is being serviced.

case canceled

Item thumbnail request has been canceled.

case invalid

Item thumbnail request completed with invalid result.

case notAvailable

Item does not have thumbnail available.

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

static var alreadyFetching: ICReturnThumbnailError.Code

Item thumbnail request is being serviced.

static var canceled: ICReturnThumbnailError.Code

Item thumbnail request has been canceled.

static var invalid: ICReturnThumbnailError.Code

Item thumbnail request completed with invalid result.

static var notAvailable: ICReturnThumbnailError.Code

Item does not have thumbnail available.

