

- Group Activities
-  SpatialTemplateElementPosition 

Structure

# SpatialTemplateElementPosition

A type that defines the position of an element in a spatial template.

visionOS 2.0+

``` source
struct SpatialTemplateElementPosition
```

## Overview

Use the `SpatialTemplateElementPosition` type to specify the position of an element along the x- and z-axes in the shared coordinate space. You place elements relative to the app’s content, which sits at the origin of the coordinate space. Specify distances in meters. The following example positions two participants one meter away from the app’s content, and on opposite sides of it:

```
struct BasicTemplate: SpatialTemplate {
    var elements: [any SpatialTemplateElement] = [
        .seat(position: .app.offsetBy(x: 0, z: 1)),
        .seat(position: .app.offsetBy(x: 0, z: -1)),
    ]
}
```

## Topics

### Getting the app’s position

static var app: SpatialTemplateElementPosition

The position of the app’s content in the shared coordinate space.

### Modifying a position

func offsetBy(x: Double, z: Double) -> SpatialTemplateElementPosition

Returns a new position at the specified distance from the origin of the shared coordinate space.

### Operators

static func == (SpatialTemplateElementPosition, SpatialTemplateElementPosition) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Custom spatial templates

Building a guessing game for visionOS

Create a team-based guessing game for visionOS using Group Activities.

protocol SpatialTemplate

An interface you use to create custom arrangements of spatial Personas in a scene.

struct SpatialTemplateSeatElement

A spatial template element that represents a seat for a participant in the activity.

protocol SpatialTemplateElement

An interface that defines an element in your spatial template.

struct SpatialTemplateElementDirection

The initial direction a participant faces when an activity starts.

protocol SpatialTemplateRole

An interface for defining roles that you assign to the participants of a group activity.

