

- Core Animation
-  CAConstraint 

Class

# CAConstraint

A representation of a single layout constraint between two layers.

Mac Catalyst 13.1+macOS 10.5+

``` source
class CAConstraint
```

## Overview

Each CAConstraint instance encapsulates one geometry relationship between two layers on the same axis.

Sibling layers are referenced by name, using the name property of each layer. The special name `superlayer` is used to refer to the layer’s superlayer.

For example, to specify that a layer should be horizontally centered in its superview you would use the following:

- Swift
- Objective-C

```
let theConstraint = CAConstraint(attribute: .midX,
                                 relativeTo: "superlayer",
                                 attribute: .midX)
```

```
```

A minimum of two relationships must be specified per axis. If you specify constraints for the left and right edges of a layer, the width will vary. If you specify constraints for the left edge and the width, the right edge of the layer will move relative to the superlayer’s frame. Often you’ll specify only a single edge constraint, the layer’s size in the same axis will be used as the second relationship.

Important

It is possible to create constraints that result in circular references to the same attributes. In cases where the layout is unable to be computed the behavior is undefined.

## Topics

### Create a New Constraint

convenience init(attribute: CAConstraintAttribute, relativeTo: String, attribute: CAConstraintAttribute, offset: CGFloat)

Creates and returns an `CAConstraint` object with the specified parameters.

convenience init(attribute: CAConstraintAttribute, relativeTo: String, attribute: CAConstraintAttribute)

Creates and returns an `CAConstraint` object with the specified parameters.

init(attribute: CAConstraintAttribute, relativeTo: String, attribute: CAConstraintAttribute, scale: CGFloat, offset: CGFloat)

Returns an `CAConstraint` object with the specified parameters. Designated initializer.

### Accessing Constraint Values

var attribute: CAConstraintAttribute

The attribute the constraint affects.

var offset: CGFloat

Offset value of the constraint attribute.

var scale: CGFloat

Scale factor of the constraint attribute.

var sourceAttribute: CAConstraintAttribute

The constraint attribute of the layer the receiver is calculated relative to

var sourceName: String

Name of the layer that the constraint is calculated relative to.

### Constants

enum CAConstraintAttribute

The constraint attribute type.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Layer Basics

class CALayer

An object that manages image-based content and allows you to perform animations on that content.

protocol CALayerDelegate

Methods your app can implement to respond to layer-related events.

protocol CALayoutManager

Methods that allow an object to manage the layout of a layer and its sublayers.

class CAConstraintLayoutManager

An object that provides a constraint-based layout manager.

protocol CAAction

An interface that allows instances to respond to actions triggered by a Core Animation layer change.

