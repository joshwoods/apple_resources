

- SwiftUI
- ScenePhase
-  ScenePhase.active 

Case

# ScenePhase.active

The scene is in the foreground and interactive.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case active
```

## Discussion

An active scene isn’t necessarily front-most. For example, a macOS window might be active even if it doesn’t currently have focus. Nevertheless, all scenes should operate normally in this phase.

An app or custom scene in this phase contains at least one active scene instance.

## See Also

### Getting scene phases

case inactive

The scene is in the foreground but should pause its work.

case background

The scene isn’t currently visible in the UI.

