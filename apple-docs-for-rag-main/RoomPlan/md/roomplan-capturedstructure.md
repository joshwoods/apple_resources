

- RoomPlan
-  CapturedStructure 

Structure

# CapturedStructure

An object that holds the results of the merger of multiple capture sessions.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct CapturedStructure
```

## Mentioned in 

Scanning the rooms of a single structure

## Overview

This structure combines the data from multiple CapturedRoom instances that a user scans in the same physical vicinity. The StructureBuilder class’s function merges the captured rooms with the capturedStructure(from:) function, which returns an object of this type.

## Topics

### Creating a captured room

init(from: any Decoder) throws

Creates a captured structure by deserializing the decoder of a prior captured structure.

### Inspecting structure details

var identifier: UUID

A unique alphanumeric value that the framework assigns the structure.

var rooms: [CapturedRoom]

An array of all the captured rooms in the structure.

var floors: [CapturedStructure.Surface]

An array of all the floors in the structure.

typealias Surface

The type a captured structure assigns to surfaces.

var doors: [CapturedStructure.Surface]

An array of all the doors in the structure.

var objects: [CapturedStructure.Object]

An array of all the objects in the structure.

typealias Object

The type a captured structure assigns to objects.

var openings: [CapturedStructure.Surface]

An array of all the openings in the structure.

var walls: [CapturedStructure.Surface]

An array of all the walls in the structure.

var windows: [CapturedStructure.Surface]

An array of all the windows in the structure.

var sections: [CapturedStructure.Section]

One or more room types that the framework identifies in the structure.

typealias Section

The type a captured structure assigns to distinct room areas.

var version: Int

A version number for the captured structure.

### Serializing a captured structure

func encode(to: any Encoder) throws

Serializes a captured structure to the specified encoder.

### Generating a USDZ file

func export(to: URL, metadataURL: URL?, modelProvider: CapturedStructure.ModelProvider?, exportOptions: CapturedStructure.USDExportOptions) throws

Produces a 3D asset from the captured structure.

typealias USDExportOptions

The type a captured structure uses to configure exports.

typealias ModelProvider

The type a captured structure uses to output sophisticated 3D models.

### Handling errors

typealias Error

Errors that can occur during a captured structure export.

## Relationships

### Conforms To

- Decodable
- Encodable
- Sendable

## See Also

### Captured Data

Merging multiple scans into a single structure

Export a 3D model that consists of multiple rooms captured in the same physical vicinity.

Scanning the rooms of a single structure

Create an AR experience that enables people to scan a building that contains multiple rooms.

struct CapturedRoom

A structure that provides the key details of a scanned room.

struct CapturedRoomData

An opaque object that holds the raw results of a scan.

Captured Object Attributes

Determine details about the objects and surfaces that the framework identifies in a scan.

