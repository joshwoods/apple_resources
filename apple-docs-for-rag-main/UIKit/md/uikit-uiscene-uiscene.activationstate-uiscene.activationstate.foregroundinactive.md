

- UIKit
- UIScene
- UIScene.ActivationState
-  UIScene.ActivationState.foregroundInactive 

Case

# UIScene.ActivationState.foregroundInactive

A state that indicates that the scene is running in the foreground but is not receiving events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
case foregroundInactive
```

## Discussion

A scene transits through the foreground-inactive state on its way to or from another state.

## See Also

### Scene States

case unattached

A state that indicates that the scene is not currently connected to your app.

case foregroundActive

A state that indicates that the scene is running in the foreground and is currently receiving events.

case background

A state that indicates that the scene is running in the background and is not onscreen.

