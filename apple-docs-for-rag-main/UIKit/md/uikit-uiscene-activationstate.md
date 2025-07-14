

- UIKit
- UIScene
-  activationState 

Instance Property

# activationState

The current execution state of the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var activationState: UIScene.ActivationState { get }
```

## Discussion

When it is running, a scene is usually in the UIScene.ActivationState.foregroundActive or UIScene.ActivationState.background state. A state may also enter other states for a short time as part of a transition.

## See Also

### Getting the scene attributes

enum ActivationState

Constants that indicate the foreground or background execution state of your app.

var title: String!

A user-visible string you supply to help users differentiate among your app’s scenes.

var subtitle: String

A string that the app displays in the title bar of a window when running in macOS.

