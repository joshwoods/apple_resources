

- RoomPlan
- CapturedRoom
-  CapturedRoom.Surface 

Structure

# CapturedRoom.Surface

A 2D area in a room that the framework identifies as a surface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct Surface
```

## Overview

A captured room (CapturedRoom) contains an arrays of surfaces that it identifies in a scan, such as its doors, openings, walls, and windows.

## Topics

### Creating a surface

init(from: any Decoder) throws

Creates a surface by deserializing the specified decoder.

### Identifying a surface

var identifier: UUID

A unique alphanumeric value that the framework assigns the surface.

var parentIdentifier: UUID?

A unique alphanumeric value that identifies a surface’s parent surface.

var category: CapturedRoom.Surface.Category

A classification that the captured room assigns the surface.

enum Category

Classifications of a surface in a captured room.

var confidence: CapturedRoom.Confidence

A level of certainty in the surface’s category.

### Positioning and sizing a surface

var transform: simd_float4x4

A matrix that defines the surface’s position and orientation in the scene.

var dimensions: simd_float3

A bounding box that contains the surface.

var story: Int

indicator for which story, level, or floor

### Shaping a surface

var completedEdges: Set&lt;CapturedRoom.Surface.Edge>

An array of edges that outline the surface.

enum Edge

An object that represents a single edge of a surface.

var curve: CapturedRoom.Surface.Curve?

An object that represents the curve of a surface.

struct Curve

An object that represents a single curve of a surface.

var polygonCorners: [simd_float3]

A 2D polygon that represents nonuniform wall heights and floor shapes.

### Serializing a surface

func encode(to: any Encoder) throws

Serializes a surface to the specified encoder.

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

enum Confidence

Levels of certainty in the classification of a particular detail in a scan.

var version: Int

A version number for the captured room.

