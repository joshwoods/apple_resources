

- RoomPlan
-  CapturedRoom 

Structure

# CapturedRoom

A structure that provides the key details of a scanned room.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct CapturedRoom
```

## Mentioned in 

Scanning the rooms of a single structure

## Overview

This structure represents the post-processed result of the room-scanning process.

Your app receives an instance of this structure through:

- The view delegate (RoomCaptureViewDelegate) callback captureView(didPresent:error:) for an app that scans rooms using the framework-provided view (RoomCaptureView).

- A room builder object (RoomBuilder) by calling capturedRoom(from:) for an app that provides its own room-scanning view, or processes the saved results of a prior scan.

With the room details, an app can provide custom features, such as rendering the room and enabling the user to modify the position of its objects. You can export the current state of the room at any time to a USDZ file by calling export(to:metadataURL:modelProvider:exportOptions:).

## Topics

### Creating a captured room

init(from: any Decoder) throws

Creates a captured room by deserializing the decoder of a previously captured room.

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

enum Confidence

Levels of certainty in the classification of a particular detail in a scan.

var version: Int

A version number for the captured room.

### Serializing a captured room

func encode(to: any Encoder) throws

Serializes a captured room to the specified encoder.

struct AttributesCodableRepresentation

A serializable set of details that describe an object in the room.

### Generating a USDZ file

func export(to: URL, exportOptions: CapturedRoom.USDExportOptions) throws

Produces a 3D asset from the captured room.

func export(to: URL, metadataURL: URL?, modelProvider: CapturedRoom.ModelProvider?, exportOptions: CapturedRoom.USDExportOptions) throws

Produces a 3D asset from the captured room with the given metadata output URL and model provider.

struct USDExportOptions

Options that determine the underlying data format of a scan export.

struct ModelProvider

A structure that assigns detailed 3D models to captured objects for an export.

### Handling errors

enum Error

Errors that can occur during a captured room export.

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

struct CapturedStructure

An object that holds the results of the merger of multiple capture sessions.

struct CapturedRoomData

An opaque object that holds the raw results of a scan.

Captured Object Attributes

Determine details about the objects and surfaces that the framework identifies in a scan.

