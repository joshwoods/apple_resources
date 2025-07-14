

- ImageCaptureCore
- ICReturnMetadataError
-  ICReturnMetadataError.Code 

Enumeration

# ICReturnMetadataError.Code

iOSiPadOSMac CatalystmacOSvisionOS

``` source
enum Code
```

## Topics

### Error Cases

case alreadyFetching

Item metadata request is being serviced.

case canceled

Item metadata request has been canceled.

case invalid

Item metadata request completed with invalid result.

case notAvailable

Item does not have metadata available.

case alreadyFetching

Item metadata request is being serviced.

case canceled

Item metadata request has been canceled.

case invalid

Item metadata request completed with invalid result.

case notAvailable

Item does not have metadata available.

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

static var alreadyFetching: ICReturnMetadataError.Code

Item metadata request is being serviced.

static var canceled: ICReturnMetadataError.Code

Item metadata request has been canceled.

static var invalid: ICReturnMetadataError.Code

Item metadata request completed with invalid result.

static var notAvailable: ICReturnMetadataError.Code

Item does not have metadata available.

