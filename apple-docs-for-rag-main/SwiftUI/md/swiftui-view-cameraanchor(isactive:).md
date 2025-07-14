

- SwiftUI
- View
-  cameraAnchor(isActive:) 

Instance Method

# cameraAnchor(isActive:)

Specifies the view that should act as the virtual camera for Apple Vision Pro 2D Persona stream.

AVKitSwiftUIvisionOS 2.0+

``` source
@MainActor
func cameraAnchor(isActive: Bool = true) -> some View
```

## Parameters 

`isActive`  

Whether or not the camera anchor is active.

You can use this value to ensure that only one camera anchor is active at a time if you want to create multiple views that could act as the anchor in your app.

## Discussion

This modifier can be used by visionOS apps to specify the placement of the virtual camera used to create a 2D stream of the user’s Persona. For example, a video conferencing app might add this modifier to the view that shows the other participants during a call. Then when the participant on visionOS looks at that view their Persona will make eye contact with the other participants on the call. The anchor will be at the center of the modified View.

```
ExampleAppVideoView()
    .cameraAnchor()
```

You might want to create multiple views with an anchor and then only activate the one that has focus.

```
struct ExampleSelfPreviewWhenFocusedView: View {
   @Environment(\.isFocused) var isFocused: Bool

   var body: some View {
       ExampleAppVideoView()
        #if os(visionOS)
            .cameraAnchor(isActive: isFocused)
        #endif
   }
}
```

Important

You should avoid creating multiple views with simultaneously active camera anchors. If multiple views with active camera anchors are found, the first created will have its parent View be used as the camera anchor, and a runtime error will be emitted.

## See Also

### Displaying media

@MainActor @preconcurrency struct CameraView

A SwiftUI view into which a video stream or an image snapshot is rendered.

@MainActor @preconcurrency struct NowPlayingView

A view that displays the system’s Now Playing interface so that the user can control audio.

@MainActor @preconcurrency struct VideoPlayer&lt;VideoOverlay> where VideoOverlay : View

A view that displays content from a player and a native user interface to control playback.

func continuityDevicePicker(isPresented: Binding&lt;Bool>, onDidConnect: ((AVContinuityDevice?) -> Void)?) -> some View

A `continuityDevicePicker` should be used to discover and connect nearby continuity device through a button interface or other form of activation. On tvOS, this presents a fullscreen continuity device picker experience when selected. The modal view covers as much the screen of `self` as possible when a given condition is true.

