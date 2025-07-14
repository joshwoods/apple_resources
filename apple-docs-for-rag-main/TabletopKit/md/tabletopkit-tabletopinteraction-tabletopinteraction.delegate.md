

- TabletopKit
- TabletopInteraction
-  TabletopInteraction.Delegate 

Protocol

# TabletopInteraction.Delegate

A protocol for objects that manage the entire flow of players interacting with equipment.

visionOS 2.0+

``` source
protocol Delegate
```

## Overview

Implement the update(interaction:) method to take an appropriate action depending on the equipment and the phase of the interaction. For example, turn a card face up if a player flips it over or toss a die when a gesture ends. Implement the `shouldAcceptInteraction(initialValue:handoffValue)` method to allow handoff interactions, to provide the initial configuration for new interactions, and to decide if a new interaction should be rejected. If `shouldAcceptInteraction(initialValue:handoffValue)` is not implemented, all handoff interactions will be rejected.

## Topics

### Taking actions

func update(interaction: TabletopInteraction)

**Required**

### Instance Methods

func shouldAcceptInteraction(initialValue: TabletopInteraction.Value, handoffValue: TabletopInteraction.Value?) -> TabletopInteraction.NewInteractionIntent

**Required** Default implementation provided.

## See Also

### Performing actions

func addAction(some TabletopAction)

func addActions(some Sequence&lt;any TabletopAction>)

func toss(equipmentID: EquipmentIdentifier, as: TossableRepresentation, linearVelocity: Vector3D?, angularVelocity: Vector3D?)

Begins a simulation of a toss of the equipment with the specificied parameters. Equipment that begins a toss in the same TabletopInteraction may interact with each other as well as the game’s boundary.

func end()

Ends the current interaction.

func cancel()

Cancels the current interaction. All actions added to the interaction will also be cancelled.

