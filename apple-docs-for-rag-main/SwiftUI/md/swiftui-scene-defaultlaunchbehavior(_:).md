

- SwiftUI
- Scene
-  defaultLaunchBehavior(\_:) 

Instance Method

# defaultLaunchBehavior(\_:)

Sets the default launch behavior for this scene.

macOS 15.0+

``` source
nonisolated
func defaultLaunchBehavior(_ behavior: SceneLaunchBehavior) -> some Scene
```

## Discussion

This behavior can be used to define if a scene is shown on application launch in the absence of any previously saved state.

On platforms that do not support multiple windows, this value is ignored.

On platforms other than macOS, there must be at least one scene that presents itself. If no scenes are defined to present, the first scene will be presented, regardless of the value provided to this modifier.

On macOS, this behavior will also be used to determine which scene is presented when clicking on the icon of a running application with no visible windows.

For example, you may wish to present a welcome window on launch of your app when there are no previous document windows being restored:

```
@main
struct MyApp: App {
    var body: some Scene {
        DocumentGroup(newDocument: MyDocument()) { configuration in
            DocumentEditor(configuration.$document)
        }

        Window("Welcome to My App", id: "welcome") {
            WelcomeView()
        }
        .defaultLaunchBehavior(.presented)
    }
}
```

The default value for all scenes if you do not apply this modifier is automatic. With that strategy, a scene will only present itself if it is the first scene defined by the app, and no other scenes have presented themselves.

## See Also

### Configuring window visibility

struct WindowVisibilityToggle

A specialized button for toggling the visibility of a window.

func restorationBehavior(SceneRestorationBehavior) -> some Scene

Sets the restoration behavior for this scene.

struct SceneLaunchBehavior

The launch behavior for a scene.

struct SceneRestorationBehavior

The restoration behavior for a scene.

func persistentSystemOverlays(Visibility) -> some Scene

Sets the preferred visibility of the non-transient system views overlaying the app.

func windowToolbarFullScreenVisibility(WindowToolbarFullScreenVisibility) -> some View

Configures the visibility of the window toolbar when the window enters full screen mode.

struct WindowToolbarFullScreenVisibility

The visibility of the window toolbar with respect to full screen mode.

