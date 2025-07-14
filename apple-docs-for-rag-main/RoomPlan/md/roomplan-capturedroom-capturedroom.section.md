

- RoomPlan
- CapturedRoom
-  CapturedRoom.Section 

Structure

# CapturedRoom.Section

An object that identifies a particular area in a captured room in relation to common types of room areas in a building.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct Section
```

## Overview

When RoomPlan recognizes a captured room as one of the common kinds of room areas, such as a living room, the framework adds an instance of this structure to the room’s sections array.

The section instance provides:

- A label type for the common area (label), such as CapturedRoom.Section.Label.livingRoom

- A center point (center), that generally locates the area within the room

- A story (story), that identifies a floor number for the area in the building

In a larger room, the framework may identify multiple types of areas, for example, a kitchen and a dining room. In that case, the `sections` array contains both, CapturedRoom.Section.Label.kitchen and CapturedRoom.Section.Label.diningRoom, and their `center` points distinguish their individual locations within the room.

## Topics

### Creating a section

init(from: any Decoder) throws

Creates a section by deserializing the given decoder.

### Describing a section

var label: CapturedRoom.Section.Label

A textual name for the section.

enum Label

Textual names for one part of a larger structure.

### Locating a section

var story: Int

The story, floor number, or level on which the section resides in a structure.

var center: simd_float3

The center position of a section.

### Serializing a section

func encode(to: any Encoder) throws

Serializes a section to the specified encoder.

## Relationships

### Conforms To

- Decodable
- Encodable
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

enum Confidence

Levels of certainty in the classification of a particular detail in a scan.

var version: Int

A version number for the captured room.

