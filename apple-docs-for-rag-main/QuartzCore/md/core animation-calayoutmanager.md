

- Core Animation
-  CALayoutManager 

Protocol

# CALayoutManager

Methods that allow an object to manage the layout of a layer and its sublayers.

Mac CatalystmacOS

``` source
protocol CALayoutManager : NSObjectProtocol
```

## Topics

### Managing Layout

func invalidateLayout(of: CALayer)

Invalidates the layout of a layer so it knows to refresh its content on the next frame.

func layoutSublayers(of: CALayer)

Override to customize layout of sublayers whenever the layer needs redrawing.

func preferredSize(of: CALayer) -> CGSize

Override to customize layer size.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- CAConstraintLayoutManager

## See Also

### Layer Basics

class CALayer

An object that manages image-based content and allows you to perform animations on that content.

protocol CALayerDelegate

Methods your app can implement to respond to layer-related events.

class CAConstraint

A representation of a single layout constraint between two layers.

class CAConstraintLayoutManager

An object that provides a constraint-based layout manager.

protocol CAAction

An interface that allows instances to respond to actions triggered by a Core Animation layer change.

