

- SwiftUI
-  SceneRestorationBehavior 

Structure

# SceneRestorationBehavior

The restoration behavior for a scene.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct SceneRestorationBehavior
```

## Overview

Use the restorationBehavior(_:) scene modifier to apply a value of this type to a Scene you define in your App declaration. The value you specify determines how the system will restore windows from a previous run of your application.

For example, you may have a scene that you do not wish to be restored on launch:

```
@main
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
        Window(id: "network-test", "Network Connection Test") {
            NetworkTestView()
        }
        .restorationBehavior(.disabled)
    }
}
```

## Topics

### Type Properties

static let automatic: SceneRestorationBehavior

The automatic behavior. The scene’s windows will be restored as defined by the underlying platform.

static let disabled: SceneRestorationBehavior

The disabled behavior. The scene’s windows will not be restored.

## Relationships

### Conforms To

- Sendable

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

func persistentSystemOverlays(Visibility) -> some Scene

Sets the preferred visibility of the non-transient system views overlaying the app.

func windowToolbarFullScreenVisibility(WindowToolbarFullScreenVisibility) -> some View

Configures the visibility of the window toolbar when the window enters full screen mode.

struct WindowToolbarFullScreenVisibility

The visibility of the window toolbar with respect to full screen mode.

