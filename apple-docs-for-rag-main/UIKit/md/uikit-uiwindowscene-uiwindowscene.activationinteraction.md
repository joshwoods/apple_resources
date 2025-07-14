

- UIKit
- UIWindowScene
-  UIWindowScene.ActivationInteraction 

Class

# UIWindowScene.ActivationInteraction

An interaction that facilitates activating a window scene when a user pinches out on the interaction’s view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class ActivationInteraction
```

## Overview

Create a UIWindowScene.ActivationInteraction object when you want to facilitate requesting scene activation when the user pinches open on a view. You initialize the interaction with a closure that the system executes when the user triggers the interaction. The closure should return a UIWindowScene.ActivationConfiguration object. You also provide an error-handler closure that the system executes if the scene activation request fails.

To request scene activation from an interaction with a UICollectionView cell, use the collectionView(_:sceneActivationConfigurationForItemAt:point:) method.

## Topics

### Creating an activation interaction

init(UIWindowScene.ActivationInteraction.ConfigurationProvider, errorHandler: (any Error) -> Void)

Creates an activation interaction.

typealias ConfigurationProvider

A type alias defining a closure that provides an activation configuration for the activation interaction.

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
- Sendable
- UIInteraction

## See Also

### Supporting types

class ActivationAction

A menu element that requests a window scene.

class ActivationConfiguration

An object that provides configuration options for a window scene request.

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

