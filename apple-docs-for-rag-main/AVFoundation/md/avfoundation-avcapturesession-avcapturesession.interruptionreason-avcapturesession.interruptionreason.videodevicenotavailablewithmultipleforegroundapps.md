

- AVFoundation
- AVCaptureSession
- AVCaptureSession.InterruptionReason
-  AVCaptureSession.InterruptionReason.videoDeviceNotAvailableWithMultipleForegroundApps 

Case

# AVCaptureSession.InterruptionReason.videoDeviceNotAvailableWithMultipleForegroundApps

An interruption caused when your app is running in Slide Over, Split View, or Picture in Picture mode on iPad.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
case videoDeviceNotAvailableWithMultipleForegroundApps
```

## Discussion

If your capture session configuration disallows accessing the camera while multitasking, the system interrupts it with this reason when a user switches to a multitasking mode like Split View. The system doesn’t interrupt your capture session with this reason if isMultitaskingCameraAccessEnabled is true.

## See Also

### Constants

case videoDeviceNotAvailableInBackground

An interruption caused by the app being sent to the background while using a camera.

case audioDeviceInUseByAnotherClient

An interruption caused by the audio hardware temporarily being made unavailable (for example, for a phone call or alarm).

case videoDeviceInUseByAnotherClient

An interruption caused by the video device temporarily being made unavailable (for example, when used by another capture session).

case videoDeviceNotAvailableDueToSystemPressure

An interruption due to system pressure, such as thermal duress.

