

- Group Activities
-  SpatialTemplateRole 

Protocol

# SpatialTemplateRole

An interface for defining roles that you assign to the participants of a group activity.

visionOS 2.0+

``` source
protocol SpatialTemplateRole : Hashable, Sendable
```

## Overview

Adopt the SpatialTemplateRole interface in a custom `enum` and use it with your custom spatial template. Roles are an optional way for you to assign a purpose to participants with a spatial Persona. For example, a spatial template for a game might define roles for the opposing teams. When a participant joins an activity, assign one of your custom roles to place them in a specific seat of your template. Seats in the template are available only to participants with spatial Personas.

The following example shows a spatial template for a table tennis game with two teams. The first four seats are for the players of the team, and the last seat is for a spectator. When participants request a role for the red or blue team, the template assigns them to the first available seat in the array with that role.

```
struct SimpleTableTennis: SpatialTemplate {
    enum Role: String, SpatialTemplateRole {
        case blueTeam
        case redTeam
    }

    var elements: [any SpatialTemplateElement] = [
        .seat(position: .app.offsetBy(x: -1, z: -3), role: Role.blueTeam),
        .seat(position: .app.offsetBy(x: -1, z:  3), role: Role.redTeam),

        .seat(position: .app.offsetBy(x:  1, z: -3), role: Role.blueTeam),
        .seat(position: .app.offsetBy(x:  1, z:  3), role: Role.redTeam),

        .seat(position: .app.offsetBy(x: -2, z:  0)),
    ]
}
```

## Topics

### Getting the role identifier

var roleIdentifier: String

The unique identifier string for the role.

**Required** Default implementation provided.

## Relationships

### Inherits From

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

struct SpatialTemplateElementPosition

A type that defines the position of an element in a spatial template.

struct SpatialTemplateElementDirection

The initial direction a participant faces when an activity starts.

