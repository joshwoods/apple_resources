

- ImageCaptureCore
- ICReturnDownloadError
-  ICReturnDownloadError.Code 

Enumeration

# ICReturnDownloadError.Code

iOSiPadOSMac CatalystmacOSvisionOS

``` source
enum Code
```

## Topics

### Enumeration Cases

case fileWritable

The destination file is not writable.

case pathInvalid

The destination path is invalid.

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

static var fileWritable: ICReturnDownloadError.Code

The destination file is not writable.

static var pathInvalid: ICReturnDownloadError.Code

The destination path is invalid.

