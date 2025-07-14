

- Group Activities
-  SpatialTemplateSeatElement 

Structure

# SpatialTemplateSeatElement

A spatial template element that represents a seat for a participant in the activity.

visionOS 2.0+

``` source
struct SpatialTemplateSeatElement
```

## Overview

Add SpatialTemplateSeatElement types to a custom SpatialTemplate to specify the placement and orientation of participants in a group activity. When an activity starts, the system places participants into the shared coordinate space and orients them according to the seat information you provide. If you associate roles with one or more seats, participants must acquire the associated role before they can occupy the corresponding seat.

Create seat elements directly from this type and add them to the elements property of your custom template. Alternatively, use the inherited seat(position:direction:role:) function to create seats, as shown in the following example, which creates two seats on either side of the app’s content along the z-axis:

```
struct BasicTemplate: SpatialTemplate {
    var elements: [any SpatialTemplateElement] = [
        .seat(position: .app.offsetBy(x: 0, z: 1)),
        .seat(position: .app.offsetBy(x: 0, z: -1)),
    ]
}
```

## Topics

### Getting the element details

let position: SpatialTemplateElementPosition

The location of the element in the shared coordinate space.

let direction: SpatialTemplateElementDirection

The initial orientation of the element in the shared coordinate space.

let role: (any SpatialTemplateRole)?

An optional role you associate with this element.

### Operators

static func == (SpatialTemplateSeatElement, SpatialTemplateSeatElement) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Initializers

init(position: SpatialTemplateElementPosition, direction: SpatialTemplateElementDirection, role: (any SpatialTemplateRole)?)

Creates a seat element with the specified position, direction, and role information.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

SpatialTemplateElement Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable
- SpatialTemplateElement

## See Also

### Custom spatial templates

Building a guessing game for visionOS

Create a team-based guessing game for visionOS using Group Activities.

protocol SpatialTemplate

An interface you use to create custom arrangements of spatial Personas in a scene.

protocol SpatialTemplateElement

An interface that defines an element in your spatial template.

struct SpatialTemplateElementPosition

A type that defines the position of an element in a spatial template.

struct SpatialTemplateElementDirection

The initial direction a participant faces when an activity starts.

protocol SpatialTemplateRole

An interface for defining roles that you assign to the participants of a group activity.

