

- ClockKit
- CLKWatchFaceLibrary
-  CLKWatchFaceLibrary.ErrorCode 

Enumeration

# CLKWatchFaceLibrary.ErrorCode

Error codes that the watch face library returns.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.0+

``` source
enum ErrorCode
```

## Topics

### Errors

case notFileURL

No file was found at the specified URL.

case invalidFile

The specified file wasn’t a valid watch face file.

case permissionDenied

The app does not have permission to read the specified file.

case faceNotAvailable

The watch face is not available on this device.

case notFileURL

No file was found at the specified URL.

case invalidFile

The specified file wasn’t a valid watch face file.

case permissionDenied

The app does not have permission to read the specified file.

case faceNotAvailable

The watch face is not available on this device.

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

### Handling Errors

class let ErrorDomain: String

The domain for errors while importing watch faces.

