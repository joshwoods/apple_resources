

- Create ML Components
- AudioReaderError
-  AudioReaderError.microphoneAuthorizationRestricted 

Case

# AudioReaderError.microphoneAuthorizationRestricted

An error that indicates that the microphone authorization status is restricted. The user is not allowed to access audio capture devices.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
case microphoneAuthorizationRestricted
```

## See Also

### Analyzing the error

case microphoneAuthorizationDenied

An error that indicates that the microphone authorization status is denied. The user has explicitly denied permission for audio capture.

case sourceDeviceNotAvailable

An error that indicates that no source devices are available.

var errorDescription: String?

A localized message describing what error occurred.

