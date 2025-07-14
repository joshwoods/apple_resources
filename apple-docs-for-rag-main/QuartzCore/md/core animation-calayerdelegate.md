

- Core Animation
-  CALayerDelegate 

Protocol

# CALayerDelegate

Methods your app can implement to respond to layer-related events.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
protocol CALayerDelegate : NSObjectProtocol
```

## Overview

You can implement the methods of this protocol to provide the layer’s content, handle the layout of sublayers, and provide custom animation actions to perform. The object that implements this protocol must be assigned to the delegate property of the layer object.

## Topics

### Providing the Layer’s Content

func display(CALayer)

Tells the delegate to implement the display process.

func draw(CALayer, in: CGContext)

Tells the delegate to implement the display process using the layer’s context.

func layerWillDraw(CALayer)

Notifies the delegate of an imminent draw.

### Laying Out Sublayers

func layoutSublayers(of: CALayer)

Tells the delegate a layer’s bounds have changed.

### Providing a Layer’s Actions

func action(for: CALayer, forKey: String) -> (any CAAction)?

Returns the default action of the action(forKey:) method.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Layer Basics

class CALayer

An object that manages image-based content and allows you to perform animations on that content.

class CAConstraint

A representation of a single layout constraint between two layers.

protocol CALayoutManager

Methods that allow an object to manage the layout of a layer and its sublayers.

class CAConstraintLayoutManager

An object that provides a constraint-based layout manager.

protocol CAAction

An interface that allows instances to respond to actions triggered by a Core Animation layer change.

