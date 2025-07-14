

- UIKit
- UIWindowScene
-  UIWindowScene.DismissalAnimation 

Enumeration

# UIWindowScene.DismissalAnimation

Constants that indicate the types of animations available for dismissing a scene’s windows.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
enum DismissalAnimation
```

## Topics

### Animation styles

case standard

The standard dismissal animations.

case commit

Animations to use when saving changes.

case decline

Animations to use when declining changes.

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

### Supporting types

class ActivationAction

A menu element that requests a window scene.

class ActivationConfiguration

An object that provides configuration options for a window scene request.

class ActivationInteraction

An interaction that facilitates activating a window scene when a user pinches out on the interaction’s view.

class ActivationRequestOptions

An object that contains information you want the system to use when activating a new window scene.

class UIWindowSceneDestructionRequestOptions

An object that contains information to use when removing a window scene from your app.

class UIWindowSceneDragInteraction

An interaction you add to a view that enables pan gestures to change the containing window scene’s position.

enum ResizingRestrictions

enum UIWindowSceneResizingRestrictions

enum PresentationStyle

The placement of a window scene relative to other scenes in the workspace.

Deprecated

