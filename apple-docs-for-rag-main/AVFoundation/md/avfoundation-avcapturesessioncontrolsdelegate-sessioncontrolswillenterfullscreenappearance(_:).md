

- AVFoundation
- AVCaptureSessionControlsDelegate
-  sessionControlsWillEnterFullscreenAppearance(\_:) 

Instance Method

# sessionControlsWillEnterFullscreenAppearance(\_:)

Tells the delegate when a capture session’s controls are about to enter a fullscreen appearance.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
func sessionControlsWillEnterFullscreenAppearance(_ session: AVCaptureSession)
```

**Required**

## Parameters 

`session`  

The capture session with controls that are entering a fullscreen appearance.

## Discussion

When controls enter a fullscreen appearance, your app should hide portions of its user interface, including duplicative or unnecessary elements. Few onscreen elements should be visible so people can focus on their control interactions while viewing the camera preview unobstructed.

## See Also

### Responding to control events

func sessionControlsDidBecomeActive(AVCaptureSession)

Tells the delegate when a capture session’s controls become active and available for interaction.

**Required**

func sessionControlsWillExitFullscreenAppearance(AVCaptureSession)

Tells the delegate when a capture session’s controls are about to exit a fullscreen appearance.

**Required**

func sessionControlsDidBecomeInactive(AVCaptureSession)

Tells the delegate when a capture session’s controls become inactive and unavailable for interaction.

**Required**

