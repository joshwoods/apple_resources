

- Group Activities
-  SpatialTemplateElementDirection 

Structure

# SpatialTemplateElementDirection

The initial direction a participant faces when an activity starts.

visionOS 2.0+

``` source
struct SpatialTemplateElementDirection
```

## Overview

A `SpatialTemplateElementDirection` type indicates where a participant faces at the start of an activity. You might configure participants to face your app’s content, another participant, or an arbitrary point in the shared coordinate system. You can also modify an existing direction value by adding an arbitrary amount of additional rotation. When a participant joins an activity, the system sets the initial orientation of their spatial Persona to the direction assigned to their seat position. If you don’t specify an initial direction for a seat, the participant faces your app’s content.

The following example creates a spatial template for a table tennis game with four participants and a spectator. The template places the red and blue teams at opposite ends of the table along the z-axis, and each person faces the app’s content along that axis. The final participant sits to the side of the table to watch the game.

```
struct TableTennis: SpatialTemplate {
    enum Role: String, SpatialTemplateRole {
        case blueTeam
        case redTeam
    }

    var elements: [any SpatialTemplateElement] = [
        .seat(position: .app.offsetBy(x: -1, z: -3), direction: .alignedWith(appAxis: .z), role: Role.blueTeam),
        .seat(position: .app.offsetBy(x: -1, z:  3), direction: .alignedWith(appAxis: .z), role: Role.redTeam),

        .seat(position: .app.offsetBy(x:  1, z: -3), direction: .alignedWith(appAxis: .z), role: Role.blueTeam),
        .seat(position: .app.offsetBy(x:  1, z:  3), direction: .alignedWith(appAxis: .z), role: Role.redTeam),

        .seat(position: .app.offsetBy(x: -2, z:  0))
    ]
}
```

## Topics

### Looking at a specific location

static func lookingAt(any SpatialTemplateElement) -> SpatialTemplateElementDirection

Creates a direction that orients the participant to face another template element.

static func lookingAt(SpatialTemplateElementPosition) -> SpatialTemplateElementDirection

Creates a direction that orients the participant to face the specified point in the shared coordinate space.

### Looking along an axis

static func alignedWith(appAxis: SpatialTemplateElementAxis) -> SpatialTemplateElementDirection

Creates a direction that orients the participant to look along the specified axis in the direction of the app’s content.

struct SpatialTemplateElementAxis

An axis to use when aligning elements in a spatial template.

### Rotating the element

func rotatedBy(Angle2D) -> SpatialTemplateElementDirection

Returns a new direction structure that adds the specified rotation angle to the current direction’s value.

### Operators

static func + (SpatialTemplateElementDirection, Angle2D) -> SpatialTemplateElementDirection

Adds the y-axis rotations for the specified values together and returns a new structure with the result.

static func == (SpatialTemplateElementDirection, SpatialTemplateElementDirection) -> Bool

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

struct SpatialTemplateElementPosition

A type that defines the position of an element in a spatial template.

protocol SpatialTemplateRole

An interface for defining roles that you assign to the participants of a group activity.

