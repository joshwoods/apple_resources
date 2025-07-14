

- SwiftUI
- Scene
-  persistentSystemOverlays(\_:) 

Instance Method

# persistentSystemOverlays(\_:)

Sets the preferred visibility of the non-transient system views overlaying the app.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func persistentSystemOverlays(_ preferredVisibility: Visibility) -> some Scene
```

## Discussion

Use this modifier to influence the appearance of system overlays in your app. The behavior varies by platform.

In iOS, the following example hides every persistent system overlay. In visionOS 2 and later, the SharePlay Indicator hides if the scene is shared through SharePlay, or not shared at all. During screen sharing, the indicator always remains visible. The Home indicator doesn’t appear without specific user intent when you set visibility to `hidden`. For a WindowGroup, the modifier affects the visibility of the window chrome. For an ImmersiveSpace, it affects the Home indicator.

```
struct ImmersiveView: View {
    var body: some View {
        Text("Maximum immersion")
            .persistentSystemOverlays(.hidden)
    }
}
```

Note

You can indicate a preference with this modifier, but the system might or might not be able to honor that preference.

Affected non-transient system views can include, but are not limited to:

- The Home indicator.

- The SharePlay indicator.

- The Multitasking Controls button and Picture in Picture on iPad.

## See Also

### Configuring window visibility

struct WindowVisibilityToggle

A specialized button for toggling the visibility of a window.

func defaultLaunchBehavior(SceneLaunchBehavior) -> some Scene

Sets the default launch behavior for this scene.

func restorationBehavior(SceneRestorationBehavior) -> some Scene

Sets the restoration behavior for this scene.

struct SceneLaunchBehavior

The launch behavior for a scene.

struct SceneRestorationBehavior

The restoration behavior for a scene.

func windowToolbarFullScreenVisibility(WindowToolbarFullScreenVisibility) -> some View

Configures the visibility of the window toolbar when the window enters full screen mode.

struct WindowToolbarFullScreenVisibility

The visibility of the window toolbar with respect to full screen mode.

