

- Core Animation
-  CAAction 

Protocol

# CAAction

An interface that allows instances to respond to actions triggered by a Core Animation layer change.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
protocol CAAction
```

## Overview

When queried with an action identifier (a key path, an external action name, or a predefined action identifier) a layer returns the appropriate action object–which must implement the CAAction protocol–and sends it a run(forKey:object:arguments:) message.

## Topics

### Responding to an action

func run(forKey: String, object: Any, arguments: [AnyHashable : Any]?)

Called to trigger the action specified by the identifier.

**Required**

## Relationships

### Conforming Types

- CAAnimation
- CAAnimationGroup
- CABasicAnimation
- CAKeyframeAnimation
- CAPropertyAnimation
- CASpringAnimation
- CATransition

## See Also

### Layer Basics

class CALayer

An object that manages image-based content and allows you to perform animations on that content.

protocol CALayerDelegate

Methods your app can implement to respond to layer-related events.

class CAConstraint

A representation of a single layout constraint between two layers.

protocol CALayoutManager

Methods that allow an object to manage the layout of a layer and its sublayers.

class CAConstraintLayoutManager

An object that provides a constraint-based layout manager.

