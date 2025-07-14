

- UIKit
- UIWindowScene
-  UIWindowScene.ActivationConfiguration 

Class

# UIWindowScene.ActivationConfiguration

An object that provides configuration options for a window scene request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
class ActivationConfiguration
```

## Overview

Use a UIWindowScene.ActivationConfiguration object to request a new window scene from the system. An activation configuration requires a NSUserActivity object that represents the scene’s content. You can specify a preferred presentation style for the new scene by including an optional UIWindowScene.ActivationRequestOptions object. The system automatically animates the transition to the new scene, but you can customize the transition by providing an optional targeted preview.

To request scene activation from a view interaction, use an instance of this class with UIWindowScene.ActivationInteraction. To request scene activation from a context menu, use an instance of this class with UIWindowScene.ActivationAction.

## Topics

### Creating an activation configuration

convenience init(userActivity: NSUserActivity, options: UIWindowScene.ActivationRequestOptions?, preview: UITargetedPreview?)

Creates an activation configuration.

### Getting information about the activation configuration

var userActivity: NSUserActivity

The user activity used to request a scene.

var options: UIWindowScene.ActivationRequestOptions?

Options for customizing the scene request.

class ActivationRequestOptions

An object that contains information you want the system to use when activating a new window scene.

var preview: UITargetedPreview?

An optional targeted preview that the system uses to animate the transition to the new scene.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Supporting types

class ActivationAction

A menu element that requests a window scene.

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

enum PresentationStyle

The placement of a window scene relative to other scenes in the workspace.

Deprecated

