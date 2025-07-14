

- Group Activities
- SystemCoordinator
- SystemCoordinator.ParticipantState
-  SystemCoordinator.ParticipantState.Seat 

Structure

# SystemCoordinator.ParticipantState.Seat

A seat assigned to a single participant in a spatial template.

visionOS 2.0+

``` source
struct Seat
```

## Overview

You can use this structure to inspect the initial position of a participant in your group activity and place UI elements near them.

## Topics

### Operators

static func == (SystemCoordinator.ParticipantState.Seat, SystemCoordinator.ParticipantState.Seat) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let pose: Pose3D

The position and rotation of the seat.

let role: (any SpatialTemplateRole)?

The role attached to this seat, if any.

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

