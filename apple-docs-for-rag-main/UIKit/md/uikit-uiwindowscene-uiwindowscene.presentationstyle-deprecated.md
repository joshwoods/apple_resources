

- UIKit
- UIWindowScene
-  UIWindowScene.PresentationStyle Deprecated

Enumeration

# UIWindowScene.PresentationStyle

The placement of a window scene relative to other scenes in the workspace.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedtvOS 15.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
enum PresentationStyle
```

## Topics

### Constants

case automatic

The system determines the most appropriate style.

case prominent

Presents prominently above others in the current space.

case standard

The default style of the system.

### Initializers

init?(rawValue: UInt)

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

enum DismissalAnimation

Constants that indicate the types of animations available for dismissing a scene’s windows.

class UIWindowSceneDragInteraction

An interaction you add to a view that enables pan gestures to change the containing window scene’s position.

enum ResizingRestrictions

enum UIWindowSceneResizingRestrictions

