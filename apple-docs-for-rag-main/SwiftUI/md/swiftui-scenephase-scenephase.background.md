

- SwiftUI
- ScenePhase
-  ScenePhase.background 

Case

# ScenePhase.background

The scene isn’t currently visible in the UI.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case background
```

## Discussion

Do as little as possible in a scene that’s in the `background` phase. The `background` phase can precede termination, so do any cleanup work immediately upon entering this state. For example, close any open files and network connections. However, a scene can also return to the ScenePhase.active phase from the background.

Expect an app that enters the `background` phase to terminate.

## See Also

### Getting scene phases

case active

The scene is in the foreground and interactive.

case inactive

The scene is in the foreground but should pause its work.

