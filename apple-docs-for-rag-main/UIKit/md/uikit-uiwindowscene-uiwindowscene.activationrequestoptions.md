

- UIKit
- UIWindowScene
-  UIWindowScene.ActivationRequestOptions 

Class

# UIWindowScene.ActivationRequestOptions

An object that contains information you want the system to use when activating a new window scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
class ActivationRequestOptions
```

## Overview

Create a UIWindowScene.ActivationRequestOptions object before you activate a scene using the activateSceneSession(for:errorHandler:) (Swift) or activateSceneSessionForRequest:errorHandler: (Objective-C) method of UIApplication. Use this object to specify the preferred presentation style of the new scene.

## Topics

### Positioning windows

var placement: (any UIWindowScenePlacement)?

The placement you prefer when the system activates the window scene.

protocol UIWindowScenePlacement

The placement of a window scene in the workspace.

struct UIWindowSceneProminentPlacement

A placement that indicates the system should present the window more prominently than others in the space.

struct UIWindowSceneStandardPlacement

A placement that indicates the system should present the window using the default style of the system in the space.

struct UIWindowScenePushPlacement

A placement that indicates the system needs to present the window by pushing it onto another window.

### Deprecated

var preferredPresentationStyle: UIWindowScene.PresentationStyle

The presentation style of the window scene.

Deprecated

struct UIWindowSceneReplacePlacementDeprecated

## Relationships

### Inherits From

- UIScene.ActivationRequestOptions

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Supporting types

class ActivationAction

A menu element that requests a window scene.

class ActivationConfiguration

An object that provides configuration options for a window scene request.

class ActivationInteraction

An interaction that facilitates activating a window scene when a user pinches out on the interaction’s view.

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

