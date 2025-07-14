

- RoomPlan
- CapturedStructure
-  CapturedStructure.Surface 

Type Alias

# CapturedStructure.Surface

The type a captured structure assigns to surfaces.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
typealias Surface = CapturedRoom.Surface
```

## See Also

### Inspecting structure details

var identifier: UUID

A unique alphanumeric value that the framework assigns the structure.

var rooms: [CapturedRoom]

An array of all the captured rooms in the structure.

var floors: [CapturedStructure.Surface]

An array of all the floors in the structure.

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

