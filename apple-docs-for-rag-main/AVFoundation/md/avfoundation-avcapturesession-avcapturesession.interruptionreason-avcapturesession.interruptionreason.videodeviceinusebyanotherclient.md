

- AVFoundation
- AVCaptureSession
- AVCaptureSession.InterruptionReason
-  AVCaptureSession.InterruptionReason.videoDeviceInUseByAnotherClient 

Case

# AVCaptureSession.InterruptionReason.videoDeviceInUseByAnotherClient

An interruption caused by the video device temporarily being made unavailable (for example, when used by another capture session).

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
case videoDeviceInUseByAnotherClient
```

## See Also

### Constants

case videoDeviceNotAvailableInBackground

An interruption caused by the app being sent to the background while using a camera.

case audioDeviceInUseByAnotherClient

An interruption caused by the audio hardware temporarily being made unavailable (for example, for a phone call or alarm).

case videoDeviceNotAvailableWithMultipleForegroundApps

An interruption caused when your app is running in Slide Over, Split View, or Picture in Picture mode on iPad.

case videoDeviceNotAvailableDueToSystemPressure

An interruption due to system pressure, such as thermal duress.

