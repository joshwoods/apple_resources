

- UIKit
- UIWindowScene
-  UIWindowScene.ActivationAction 

Class

# UIWindowScene.ActivationAction

A menu element that requests a window scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class ActivationAction
```

## Overview

Create a UIWindowScene.ActivationAction object to facilitate activating a new window scene from a menu item. You initialize the action with a closure that the system executes when a user selects the item. The closure should return a UIWindowScene.ActivationConfiguration object. You can specify an alternate action to display on iPhone and apps that don’t support multiple windows.

## Topics

### Creating an activation action

convenience init(title: String?, subtitle: String?, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, alternate: UIAction?, UIWindowScene.ActivationAction.ConfigurationProvider)

Creates an activation action using the specified parameters.

typealias ConfigurationProvider

A type alias defining a closure that provides an activation configuration for the activation action.

### Getting information about the activation action

var title: String!

The action’s title.

## Relationships

### Inherits From

- UIAction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable
- UIAccessibilityIdentification
- UIMenuLeaf

## See Also

### Supporting types

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

enum PresentationStyle

The placement of a window scene relative to other scenes in the workspace.

Deprecated

