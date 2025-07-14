

- SwiftUI
-  SceneLaunchBehavior 

Structure

# SceneLaunchBehavior

The launch behavior for a scene.

macOS 15.0+

``` source
struct SceneLaunchBehavior
```

## Overview

Use the defaultLaunchBehavior(_:) modifier to apply a value of this type to a Scene you specify in your App. The value you specify determines how the system will present the scene in the absense of any previously restored scenes on launch of your application.

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

## Topics

### Type Properties

static let automatic: SceneLaunchBehavior

The automatic behavior.

static let presented: SceneLaunchBehavior

The presented behavior. The scene will present itself in the absence of any previously restored scenes.

static let suppressed: SceneLaunchBehavior

The suppressed behavior. The scene will not present itself in the absence of any previously restored scenes.

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

struct SceneRestorationBehavior

The restoration behavior for a scene.

func persistentSystemOverlays(Visibility) -> some Scene

Sets the preferred visibility of the non-transient system views overlaying the app.

func windowToolbarFullScreenVisibility(WindowToolbarFullScreenVisibility) -> some View

Configures the visibility of the window toolbar when the window enters full screen mode.

struct WindowToolbarFullScreenVisibility

The visibility of the window toolbar with respect to full screen mode.

