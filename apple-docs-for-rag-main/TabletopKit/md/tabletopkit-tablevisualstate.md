

- TabletopKit
-  TableVisualState 

Structure

# TableVisualState

A structure that represents the appearance of an object on the table.

visionOS 2.0+

``` source
struct TableVisualState
```

## Topics

### Representing collision states

var contacts: some Sequence&lt;TableVisualState.Contact>

Returns all contacts for the current update of the physics simulation.

func contacts&lt;E>(of: E.Type) -> some Sequence&lt;TableVisualState.Contact> 

Returns all contacts for the current update of the physics simulation for a specified equipment type.

struct Contact

An object that represents the contact of a collision during a simulation of tossable equipment.

### Representing 2D states

struct Point2D

An object that represents a point on the XZ plane.

struct Pose2D

An object that represents a 2D position and orientation on the XZ plane.

### Representing 3D states

struct OrientedRect3D

An object that represents the position and orientation of a 3D rectangle.

func bounds(forEquipment: some Equipment) -> TableVisualState.OrientedRect3D?

func bounds(matching: EquipmentIdentifier) -> TableVisualState.OrientedRect3D?

func goalBounds(forEquipment: some Equipment) -> TableVisualState.OrientedRect3D?

func goalBounds(matching: EquipmentIdentifier) -> TableVisualState.OrientedRect3D?

var tableBounds: TableVisualState.OrientedRect3D?

### Representing seat states

func pose(forSeat: some TableSeat) -> Pose3D?

func pose(matching: TableSeatIdentifier) -> Pose3D?

## See Also

### Interactions

class TabletopInteraction

A protocol for objects that manage the entire flow of players interacting with equipment.

struct TossableRepresentation

An object that represents geometric shapes that the player can throw during gameplay, such as dice.

struct TableSnapshot

A snapshot of the current state of the table.

struct TableCursor

A visual indicator that represents the destination of player interactions with equipment.

struct TableCursorIdentifier

A unique identifier for cursors.

