

- Create ML Components
- VideoReaderError
-  VideoReaderError.missingVideoTrack(\_:) 

Case

# VideoReaderError.missingVideoTrack(\_:)

An error that indicates that the VideoReader cannot find a video track.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
case missingVideoTrack(URL)
```

## See Also

### Analyzing the error

case cameraAuthorizationDenied

An error that indicates that the camera authorization status is denied. The user has explicitly denied permission for media capture.

case cameraAuthorizationRestricted

An error that indicates that the camera authorization status is restricted. The user is not allowed to access media capture devices.

case frameRateNotSupported(Double)

An error that indicates that the frame rate is not supported by the input camera.

case sourceCameraNotAvailable

An error that indicates that no cameras are available.

var errorDescription: String?

A localized message describing what error occurred.

