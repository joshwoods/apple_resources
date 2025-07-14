

- RealityKit
- RealityViewDefaultPlaceholder
-  realityViewCameraControls(\_:) 

Instance Method

# realityViewCameraControls(\_:)

Adds gestures that control the position and direction of a virtual camera.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
@MainActor @preconcurrency
func realityViewCameraControls(_ controls: CameraControls) -> some View
```

## Discussion

You can use a drag gesture from a mouse, trackpad, or screen touches with iOS and iPadOS devices to `.tilt`, `.pan`, `.orbit`, or `.dolly` a virtual camera.

