

- AVFoundation
- AVCaptureSessionControlsDelegate
-  sessionControlsDidBecomeActive(\_:) 

Instance Method

# sessionControlsDidBecomeActive(\_:)

Tells the delegate when a capture session’s controls become active and available for interaction.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
func sessionControlsDidBecomeActive(_ session: AVCaptureSession)
```

**Required**

## Parameters 

`session`  

The capture session with active controls.

## See Also

### Responding to control events

func sessionControlsWillEnterFullscreenAppearance(AVCaptureSession)

Tells the delegate when a capture session’s controls are about to enter a fullscreen appearance.

**Required**

func sessionControlsWillExitFullscreenAppearance(AVCaptureSession)

Tells the delegate when a capture session’s controls are about to exit a fullscreen appearance.

**Required**

func sessionControlsDidBecomeInactive(AVCaptureSession)

Tells the delegate when a capture session’s controls become inactive and unavailable for interaction.

**Required**

