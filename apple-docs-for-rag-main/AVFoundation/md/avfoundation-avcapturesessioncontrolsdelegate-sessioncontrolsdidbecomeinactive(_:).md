

- AVFoundation
- AVCaptureSessionControlsDelegate
-  sessionControlsDidBecomeInactive(\_:) 

Instance Method

# sessionControlsDidBecomeInactive(\_:)

Tells the delegate when a capture session’s controls become inactive and unavailable for interaction.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
func sessionControlsDidBecomeInactive(_ session: AVCaptureSession)
```

**Required**

## Parameters 

`session`  

The capture session with inactive controls.

## See Also

### Responding to control events

func sessionControlsDidBecomeActive(AVCaptureSession)

Tells the delegate when a capture session’s controls become active and available for interaction.

**Required**

func sessionControlsWillEnterFullscreenAppearance(AVCaptureSession)

Tells the delegate when a capture session’s controls are about to enter a fullscreen appearance.

**Required**

func sessionControlsWillExitFullscreenAppearance(AVCaptureSession)

Tells the delegate when a capture session’s controls are about to exit a fullscreen appearance.

**Required**

