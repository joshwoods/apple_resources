

- SwiftUI
-  ScenePhase 

Enumeration

# ScenePhase

An indication of a scene’s operational state.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum ScenePhase
```

## Mentioned in 

Migrating to the SwiftUI life cycle

## Overview

The system moves your app’s Scene instances through phases that reflect a scene’s operational state. You can trigger actions when the phase changes. Read the current phase by observing the scenePhase value in the Environment:

```
@Environment(\.scenePhase) private var scenePhase
```

How you interpret the value depends on where it’s read from. If you read the phase from inside a View instance, you obtain a value that reflects the phase of the scene that contains the view. The following example uses the onChange(of:initial:_:) method to enable a timer whenever the enclosing scene enters the ScenePhase.active phase and disable the timer when entering any other phase:

```
struct MyView: View {
    @ObservedObject var model: DataModel
    @Environment(\.scenePhase) private var scenePhase

    var body: some View {
        TimerView()
            .onChange(of: scenePhase) {
                model.isTimerRunning = (scenePhase == .active)
            }
    }
}
```

If you read the phase from within an App instance, you obtain an aggregate value that reflects the phases of all the scenes in your app. The app reports a value of ScenePhase.active if any scene is active, or a value of ScenePhase.inactive when no scenes are active. This includes multiple scene instances created from a single scene declaration; for example, from a WindowGroup. When an app enters the ScenePhase.background phase, expect the app to terminate soon after. You can use that opportunity to free any resources:

```
@main
struct MyApp: App {
    @Environment(\.scenePhase) private var scenePhase

    var body: some Scene {
        WindowGroup {
            MyRootView()
        }
        .onChange(of: scenePhase) {
            if scenePhase == .background {
                // Perform cleanup when all scenes within
                // MyApp go to the background.
            }
        }
    }
}
```

## Topics

### Getting scene phases

case active

The scene is in the foreground and interactive.

case inactive

The scene is in the foreground but should pause its work.

case background

The scene isn’t currently visible in the UI.

## Relationships

### Conforms To

- Comparable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Monitoring scene life cycle

var scenePhase: ScenePhase

The current phase of the scene.

