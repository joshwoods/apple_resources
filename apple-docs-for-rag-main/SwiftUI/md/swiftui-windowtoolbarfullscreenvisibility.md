

- SwiftUI
-  WindowToolbarFullScreenVisibility 

Structure

# WindowToolbarFullScreenVisibility

The visibility of the window toolbar with respect to full screen mode.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct WindowToolbarFullScreenVisibility
```

## Overview

Use values of this type in conjunction with the windowToolbarFullScreenVisibility(_:) modifier to configure how the window toolbar displays itself when the window enters full screen mode.

For example, you can specify that the window toolbar should be hidden by default, and only show when the mouse moves into the area occupied by the menu bar:

```
struct RootView: View {
    var body: some View {
        ContentView()
            .toolbar {
                ...
            }
            .windowToolbarFullScreenVisibility(.onHover)
    }
}
```

## Topics

### Type Properties

static let automatic: WindowToolbarFullScreenVisibility

The window toolbar visibility will be defined by the system default behavior.

static let onHover: WindowToolbarFullScreenVisibility

Hide the window toolbar in full screen mode by default. It will reveal itself when the mouse moves into the area occupied by the menu bar.

static let visible: WindowToolbarFullScreenVisibility

Prefer to show window toolbar when the window is in full screen mode.

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

struct SceneRestorationBehavior

The restoration behavior for a scene.

func persistentSystemOverlays(Visibility) -> some Scene

Sets the preferred visibility of the non-transient system views overlaying the app.

func windowToolbarFullScreenVisibility(WindowToolbarFullScreenVisibility) -> some View

Configures the visibility of the window toolbar when the window enters full screen mode.

