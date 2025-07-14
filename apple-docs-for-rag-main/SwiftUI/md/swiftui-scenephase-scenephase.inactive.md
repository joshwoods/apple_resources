

- SwiftUI
- ScenePhase
-  ScenePhase.inactive 

Case

# ScenePhase.inactive

The scene is in the foreground but should pause its work.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case inactive
```

## Discussion

A scene in this phase doesn’t receive events and should pause timers and free any unnecessary resources. The scene might be completely hidden in the user interface or otherwise unavailable to the user. In macOS, scenes only pass through this phase temporarily on their way to the ScenePhase.background phase.

An app or custom scene in this phase contains no scene instances in the ScenePhase.active phase.

## See Also

### Getting scene phases

case active

The scene is in the foreground and interactive.

case background

The scene isn’t currently visible in the UI.

