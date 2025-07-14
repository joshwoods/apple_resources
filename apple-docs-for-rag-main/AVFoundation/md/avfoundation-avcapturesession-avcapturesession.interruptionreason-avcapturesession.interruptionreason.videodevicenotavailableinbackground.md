

- AVFoundation
- AVCaptureSession
- AVCaptureSession.InterruptionReason
-  AVCaptureSession.InterruptionReason.videoDeviceNotAvailableInBackground 

Case

# AVCaptureSession.InterruptionReason.videoDeviceNotAvailableInBackground

An interruption caused by the app being sent to the background while using a camera.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
case videoDeviceNotAvailableInBackground
```

## Discussion

Camera usage is prohibited while in the background. If you attempt to start running a camera while in the background, the capture session sends an wasInterruptedNotification with this interruption reason. If you don’t explicitly call the stopRunning() method, your startRunning() request is preserved, and when your app comes back to foreground, you receive interruptionEndedNotification and your session starts running.

## See Also

### Constants

case audioDeviceInUseByAnotherClient

An interruption caused by the audio hardware temporarily being made unavailable (for example, for a phone call or alarm).

case videoDeviceInUseByAnotherClient

An interruption caused by the video device temporarily being made unavailable (for example, when used by another capture session).

case videoDeviceNotAvailableWithMultipleForegroundApps

An interruption caused when your app is running in Slide Over, Split View, or Picture in Picture mode on iPad.

case videoDeviceNotAvailableDueToSystemPressure

An interruption due to system pressure, such as thermal duress.

