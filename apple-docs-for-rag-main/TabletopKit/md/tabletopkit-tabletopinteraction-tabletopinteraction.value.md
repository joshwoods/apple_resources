

- TabletopKit
- TabletopInteraction
-  TabletopInteraction.Value 

Structure

# TabletopInteraction.Value

A structure that provides the details about an interaction, such as the phase of the gesture and position of the equipment.

visionOS 2.0+

``` source
struct Value
```

## Topics

### Getting information about the equipment and game

var startingEquipmentID: EquipmentIdentifier

The equipment the interaction was started with

var controlledEquipmentID: EquipmentIdentifier

The equipment the interaction is currently controlling

var allowedDestinations: TabletopInteraction.AllowedDestinations

The allowed destinations that this interaction can target

Deprecated

### Getting the phases

var gesturePhase: TabletopInteraction.Value.Phase?

the current phase of the gesture

Deprecated

var phase: TabletopInteraction.Value.Phase

the current phase of the overall interaction

enum Phase

The stages of players interacting with equipment on the table.

### Getting the proposed locations

var proposedDestination: TabletopInteraction.Destination?

The proposed destination of the main interaction object, computed from the current pose of the object. During a toss simulation, the proposed destination is only updated if there is only one tossed equipment and it is the currently controlled equipment.

var proposedFlip: Bool

Was the object flipped from the start of this interaction

### Getting the position and location

var pose: Pose3D

The current pose of the main interaction object

var locationOnTable: TableVisualState.Point2D?

The 2D location of the main interaction object

var endLocation: Point3D?

The expected end location

var endLocationOnTable: TableVisualState.Point2D?

The expected end 2D location of the main interaction object

### Getting identifiers

var id: TabletopInteraction.Value.ID

Identifier to recognize different interactions from one another

var playerID: PlayerIdentifier

The player who is performing the interaction

### Structures

struct Gesture

A structure that provides details specific to a gesture driven interaction.

### Instance Properties

var configuration: TabletopInteraction.Configuration

The configuration of this interaction

var gesture: TabletopInteraction.Value.Gesture?

If this is interaction is currently gesture driven, contains gesture specific additional information

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Getting the value of the interaction

var value: TabletopInteraction.Value

The current value belonging to this interaction.

