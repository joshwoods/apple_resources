

- RoomPlan
- CapturedRoom
-  CapturedRoom.Object 

Structure

# CapturedRoom.Object

A 3D area in a room that the framework identifies as an object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct Object
```

## Overview

A captured room contains an array of this type for the objects (objects) it identifies.

## Topics

### Creating an object

init(from: any Decoder) throws

Creates an object by deserializing the specified decoder.

### Identifying an object

var identifier: UUID

A unique alphanumeric value that the framework assigns the object.

var parentIdentifier: UUID?

A unique alphanumeric value that identifies the object’s parent object or surface.

var category: CapturedRoom.Object.Category

A classification that the captured room assigns the object.

enum Category

Classifications of an object in a captured room.

var confidence: CapturedRoom.Confidence

A level of certainty in the object’s category.

### Positioning and sizing an object

var transform: simd_float4x4

A matrix that defines the object’s position and orientation in the room.

var dimensions: simd_float3

A bounding box sized to the object’s extremities.

var story: Int

The floor number or level on which the object resides.

### Describing an object

var attributes: [any CapturedRoomAttribute]

A collection of details that describe a particular object in the room.

func attribute&lt;T>(of: T.Type) -> T?

Checks an object for specific attribute types.

### Serializing an object

func encode(to: any Encoder) throws

Serializes an object to the specified encoder.

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

enum Confidence

Levels of certainty in the classification of a particular detail in a scan.

var version: Int

A version number for the captured room.

