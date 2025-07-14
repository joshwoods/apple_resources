

- UIKit
- UIScene
- UIScene.ActivationState
-  UIScene.ActivationState.unattached 

Case

# UIScene.ActivationState.unattached

A state that indicates that the scene is not currently connected to your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
case unattached
```

## Discussion

A scene starts in the unattached state and remains in that state until the system sends a connection notification to it. A scene reenters the attached state when the user dismisses the interface from the app switcher or to reclaim its resources.

## See Also

### Scene States

case foregroundInactive

A state that indicates that the scene is running in the foreground but is not receiving events.

case foregroundActive

A state that indicates that the scene is running in the foreground and is currently receiving events.

case background

A state that indicates that the scene is running in the background and is not onscreen.

