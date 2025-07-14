

- TabletopKit
-  TableCursor 

Structure

# TableCursor

A visual indicator that represents the destination of player interactions with equipment.

visionOS 2.0+

``` source
struct TableCursor
```

## Topics

### Getting the associated interaction

var interactionID: TabletopInteraction.Identifier

The interaction id for the cursor.

### Getting the player performing the interaction

var playerID: PlayerIdentifier

The player that the cursor represents.

### Getting information about the equipment in the interaction

let controlledEquipmentPose: EquipmentPose3D

Pose relative to the the table

var hovering: TabletopInteraction.Destination?

The cursor’s current position, relative to the table or a piece of equipment.

### Getting the cursor identifier

var id: TableCursor.ID

The interaction identifier for the cursor.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Interactions

class TabletopInteraction

A protocol for objects that manage the entire flow of players interacting with equipment.

struct TossableRepresentation

An object that represents geometric shapes that the player can throw during gameplay, such as dice.

struct TableSnapshot

A snapshot of the current state of the table.

struct TableVisualState

A structure that represents the appearance of an object on the table.

struct TableCursorIdentifier

A unique identifier for cursors.

