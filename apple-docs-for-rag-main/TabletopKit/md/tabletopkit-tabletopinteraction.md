

- TabletopKit
-  TabletopInteraction 

Class

# TabletopInteraction

A protocol for objects that manage the entire flow of players interacting with equipment.

visionOS 2.0+

``` source
class TabletopInteraction
```

## Overview

Conform to the TabletopInteraction.Delegate protocol to take an appropriate action, depending on the equipment and the phase of the interaction. For example, move equipment or toss a die when a gesture ends.

```
struct MoveInteraction: TabletopInteraction.Delegate {
    func update(interaction: TabletopKit.TabletopInteraction) {
        let equipment = interaction.value.controlledEquipmentID
        guard let destination = interaction.value.proposedDestination else {
            return
        }

        if interaction.value.phase == .ended {
            interaction.addAction(.moveEquipment(matching: equipment, childOf: destination.equipmentID, pose: destination.pose))
        }
    }
}
```

To get information about the equipment that the interaction applies to, use the value property. To get the phase of the interaction or gesture, use the `Value` gesturePhase or phase properties.

Then execute actions — for example, move equipment when the phase ends — using the addAction(_:) or addActions(_:) method.

To start an interaction programmatically, use the `TabletopGame` startInteraction(onEquipmentID:) method.

## Topics

### Performing actions

protocol Delegate

A protocol for objects that manage the entire flow of players interacting with equipment.

func addAction(some TabletopAction)

func addActions(some Sequence&lt;any TabletopAction>)

func toss(equipmentID: EquipmentIdentifier, as: TossableRepresentation, linearVelocity: Vector3D?, angularVelocity: Vector3D?)

Begins a simulation of a toss of the equipment with the specificied parameters. Equipment that begins a toss in the same TabletopInteraction may interact with each other as well as the game’s boundary.

func end()

Ends the current interaction.

func cancel()

Cancels the current interaction. All actions added to the interaction will also be cancelled.

### Getting the value of the interaction

var value: TabletopInteraction.Value

The current value belonging to this interaction.

struct Value

A structure that provides the details about an interaction, such as the phase of the gesture and position of the equipment.

### Setting information about the equipment and pose

func setControlledEquipment(matching: EquipmentIdentifier)

Replace the current controlled equipment with a different one

func setPose(Pose3D)

Sets the pose of the controlled `Equipment`.

### Managing the interaction destination

func setAllowedDestinations(TabletopInteraction.AllowedDestinations)

Sets which equipment the interaction can target.

Deprecated

enum AllowedDestinations

The possible destinations of equipment in an interaction.

struct Destination

An object that represents the destination position and orientation of equipment in an interaction.

### Getting the interaction identifier

struct Identifier

A unique identifier for interactions.

### Structures

struct Configuration

A struct containing the parameters that affect the behavior of the interaction.

### Instance Methods

func setConfiguration(TabletopInteraction.Configuration)

Sets the configuration of this interaction.

### Enumerations

enum NewInteractionIntent

The possible outcomes when a new interaction is about to be started.

## See Also

### Interactions

struct TossableRepresentation

An object that represents geometric shapes that the player can throw during gameplay, such as dice.

struct TableSnapshot

A snapshot of the current state of the table.

struct TableVisualState

A structure that represents the appearance of an object on the table.

struct TableCursor

A visual indicator that represents the destination of player interactions with equipment.

struct TableCursorIdentifier

A unique identifier for cursors.

