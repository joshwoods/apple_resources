

- Group Activities
-  SpatialTemplateElement 

Protocol

# SpatialTemplateElement

An interface that defines an element in your spatial template.

visionOS 2.0+

``` source
protocol SpatialTemplateElement : Hashable, Sendable
```

## Overview

A type that adopts the SpatialTemplateElement protocol defines the location and orientation of a participant in a group activity. You don’t adopt this protocol directly in your custom types. Instead, you use types that adopt this protocol to retrieve the corresponding details.

## Topics

### Creating a seat position

static func seat(position: SpatialTemplateElementPosition, direction: SpatialTemplateElementDirection, role: (any SpatialTemplateRole)?) -> Self

Creates a seat element with the specified position, direction, and role information.

### Getting the element details

var position: SpatialTemplateElementPosition

The location of the element in the shared coordinate space.

**Required**

var direction: SpatialTemplateElementDirection

The initial orientation of the element in the shared coordinate space.

**Required**

var role: (any SpatialTemplateRole)?

An optional role you associate with this element.

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable
- Sendable

### Conforming Types

- SpatialTemplateSeatElement

## See Also

### Custom spatial templates

Building a guessing game for visionOS

Create a team-based guessing game for visionOS using Group Activities.

protocol SpatialTemplate

An interface you use to create custom arrangements of spatial Personas in a scene.

struct SpatialTemplateSeatElement

A spatial template element that represents a seat for a participant in the activity.

struct SpatialTemplateElementPosition

A type that defines the position of an element in a spatial template.

struct SpatialTemplateElementDirection

The initial direction a participant faces when an activity starts.

protocol SpatialTemplateRole

An interface for defining roles that you assign to the participants of a group activity.

