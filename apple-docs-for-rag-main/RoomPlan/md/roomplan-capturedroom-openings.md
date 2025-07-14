

- RoomPlan
- CapturedRoom
-  openings 

Instance Property

# openings

An array of openings that the framework identifies during a scan.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var openings: [CapturedRoom.Surface] { get }
```

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

