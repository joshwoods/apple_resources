

- AVFoundation
- AVCaptureSession
-  AVCaptureSession.InterruptionReason 

Enumeration

# AVCaptureSession.InterruptionReason

Constants identifying the reason a capture session was interrupted, found in an wasInterruptedNotification user info dictionary.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
enum InterruptionReason
```

## Topics

### Constants

case videoDeviceNotAvailableInBackground

An interruption caused by the app being sent to the background while using a camera.

case audioDeviceInUseByAnotherClient

An interruption caused by the audio hardware temporarily being made unavailable (for example, for a phone call or alarm).

case videoDeviceInUseByAnotherClient

An interruption caused by the video device temporarily being made unavailable (for example, when used by another capture session).

case videoDeviceNotAvailableWithMultipleForegroundApps

An interruption caused when your app is running in Slide Over, Split View, or Picture in Picture mode on iPad.

case videoDeviceNotAvailableDueToSystemPressure

An interruption due to system pressure, such as thermal duress.

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

### User-Infomation Keys

let AVCaptureSessionInterruptionSystemPressureStateKey: String

A key to retrieve a state value that indicates the system pressure level and contributing factors that caused the interruption.

let AVCaptureSessionInterruptionReasonKey: String

Key to retrieve information about a capture interruption from a wasInterruptedNotification user info dictionary.

