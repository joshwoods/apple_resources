

- SwiftUI
- View
-  continuityDevicePicker(isPresented:onDidConnect:) 

Instance Method

# continuityDevicePicker(isPresented:onDidConnect:)

A `continuityDevicePicker` should be used to discover and connect nearby continuity device through a button interface or other form of activation. On tvOS, this presents a fullscreen continuity device picker experience when selected. The modal view covers as much the screen of `self` as possible when a given condition is true.

AVKitSwiftUItvOS 17.0+

``` source
@MainActor @preconcurrency
func continuityDevicePicker(
    isPresented: Binding,
    onDidConnect: ((AVContinuityDevice?) -> Void)? = nil
) -> some View
```

## Parameters 

`isPresented`  

A `Binding` to whether the modal view is presented.

`onDidConnect`  

A closure executed when the picker successfully, connects AVContinuityDevice or nil if cancelled by a user.

## See Also

### Displaying media

@MainActor @preconcurrency struct CameraView

A SwiftUI view into which a video stream or an image snapshot is rendered.

@MainActor @preconcurrency struct NowPlayingView

A view that displays the system’s Now Playing interface so that the user can control audio.

@MainActor @preconcurrency struct VideoPlayer&lt;VideoOverlay> where VideoOverlay : View

A view that displays content from a player and a native user interface to control playback.

func cameraAnchor(isActive: Bool) -> some View

Specifies the view that should act as the virtual camera for Apple Vision Pro 2D Persona stream.

