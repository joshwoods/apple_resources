

- AVFoundation
- AVCaptureSessionControlsDelegate
-  sessionControlsWillExitFullscreenAppearance(\_:) 

Instance Method

# sessionControlsWillExitFullscreenAppearance(\_:)

Tells the delegate when a capture session’s controls are about to exit a fullscreen appearance.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
func sessionControlsWillExitFullscreenAppearance(_ session: AVCaptureSession)
```

**Required**

## Parameters 

`session`  

The capture session with controls that are exiting a fullscreen appearance.

## Discussion

When your app receives this callback, it should resume showing portions of the interface it hid when controls entered a fullscreen appearance.

The system calls this method before sessionControlsDidBecomeInactive(_:).

## See Also

### Responding to control events

func sessionControlsDidBecomeActive(AVCaptureSession)

Tells the delegate when a capture session’s controls become active and available for interaction.

**Required**

func sessionControlsWillEnterFullscreenAppearance(AVCaptureSession)

Tells the delegate when a capture session’s controls are about to enter a fullscreen appearance.

**Required**

func sessionControlsDidBecomeInactive(AVCaptureSession)

Tells the delegate when a capture session’s controls become inactive and unavailable for interaction.

**Required**

