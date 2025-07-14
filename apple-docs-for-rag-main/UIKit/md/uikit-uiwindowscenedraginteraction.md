

- UIKit
-  UIWindowSceneDragInteraction 

Class

# UIWindowSceneDragInteraction

An interaction you add to a view that enables pan gestures to change the containing window scene’s position.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
class UIWindowSceneDragInteraction
```

## Overview

Create and add this interaction to a view that you want to drag to adjust the position of your app’s window. UINavigationBar handles this automatically, so you only need to add this interaction to views in other parts of your window that you want to be draggable.

- Swift
- Objective-C

```
var windowDragInteraction = UIWindowSceneDragInteraction()
draggableView.addInteraction(windowDragInteraction)
```

```
UIWindowSceneDragInteraction *windowDragInteraction = [[UIWindowSceneDragInteraction alloc] init];
[self.draggableView addInteraction:windowDragInteraction];
```

## Topics

### Preventing gesture conflicts

var gestureForFailureRelationships: UIGestureRecognizer

The gesture that the drag interaction adds to the view hierarchy.

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

class ActivationInteraction

An interaction that facilitates activating a window scene when a user pinches out on the interaction’s view.

class ActivationRequestOptions

An object that contains information you want the system to use when activating a new window scene.

class UIWindowSceneDestructionRequestOptions

An object that contains information to use when removing a window scene from your app.

enum DismissalAnimation

Constants that indicate the types of animations available for dismissing a scene’s windows.

enum ResizingRestrictions

enum UIWindowSceneResizingRestrictions

enum PresentationStyle

The placement of a window scene relative to other scenes in the workspace.

Deprecated

