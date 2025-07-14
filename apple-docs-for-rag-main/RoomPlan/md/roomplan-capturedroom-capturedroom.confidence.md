

- RoomPlan
- CapturedRoom
-  CapturedRoom.Confidence 

Enumeration

# CapturedRoom.Confidence

Levels of certainty in the classification of a particular detail in a scan.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum Confidence
```

## Overview

The framework chooses a level of certainty in its assessment of particular room features, such as:

- The confidence in a category that the captured room assigns its surfaces, such as doors, openings, walls, windows.

- The confidence in a category that the captured room assigns its objects.

## Topics

### Creating a confidence value

init(from: any Decoder) throws

Creates a confidence value by deserializing the specified decoder.

### Assessing a confidence value

case high

A confidence value that represents a high level of certainty.

case medium

A confidence value that represents a medium level of certainty.

case low

A confidence value that represents a low level of certainty.

### Comparing confidence values

static func == (CapturedRoom.Confidence, CapturedRoom.Confidence) -> Bool

Determines whether two confidence values are equal.

static func != (Self, Self) -> Bool

Determines whether two confidence values aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Serializing a confidence value

func encode(to: any Encoder) throws

Serializes a confidence value to the specified encoder.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting room details

var identifier: UUID

A unique alphanumeric value that the framework assigns the room.

var story: Int

The story, floor number, or level on which the captured room resides within a larger structure.

var floors: [CapturedRoom.Surface]

An array of floors that the framework identifies during a scan.

struct Surface

A 2D area in a room that the framework identifies as a surface.

var doors: [CapturedRoom.Surface]

An array of doors that the framework identifies during a scan.

var objects: [CapturedRoom.Object]

An array of objects that the framework identifies during a scan.

struct Object

A 3D area in a room that the framework identifies as an object.

var openings: [CapturedRoom.Surface]

An array of openings that the framework identifies during a scan.

var walls: [CapturedRoom.Surface]

An array of walls that the framework identifies during a scan.

var windows: [CapturedRoom.Surface]

An array of windows that the framework identifies during a scan.

var sections: [CapturedRoom.Section]

One or more room types that the framework observes in the room.

struct Section

An object that identifies a particular area in a captured room in relation to common types of room areas in a building.

var version: Int

A version number for the captured room.

