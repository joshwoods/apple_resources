

- UIKit
- UIScene
-  UIScene.ActivationState 

Enumeration

# UIScene.ActivationState

Constants that indicate the foreground or background execution state of your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
enum ActivationState
```

## Topics

### Scene States

case unattached

A state that indicates that the scene is not currently connected to your app.

case foregroundInactive

A state that indicates that the scene is running in the foreground but is not receiving events.

case foregroundActive

A state that indicates that the scene is running in the foreground and is currently receiving events.

case background

A state that indicates that the scene is running in the background and is not onscreen.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the scene attributes

var activationState: UIScene.ActivationState

The current execution state of the scene.

var title: String!

A user-visible string you supply to help users differentiate among your app’s scenes.

var subtitle: String

A string that the app displays in the title bar of a window when running in macOS.

