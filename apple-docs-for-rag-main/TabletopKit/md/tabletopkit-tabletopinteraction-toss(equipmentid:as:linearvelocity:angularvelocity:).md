

- TabletopKit
- TabletopInteraction
-  toss(equipmentID:as:linearVelocity:angularVelocity:) 

Instance Method

# toss(equipmentID:as:linearVelocity:angularVelocity:)

Begins a simulation of a toss of the equipment with the specificied parameters. Equipment that begins a toss in the same TabletopInteraction may interact with each other as well as the game’s boundary.

visionOS 2.0+

``` source
func toss(
    equipmentID: EquipmentIdentifier,
    as representation: TossableRepresentation,
    linearVelocity: Vector3D? = nil,
    angularVelocity: Vector3D? = nil
)
```

## Parameters 

`equipmentID`  

The equipment ID to use in the toss simulation.

`representation`  

The representation that the toss simulation will treat the equipment as.

`linearVelocity`  

The linear velocity the toss begins with. If nil, the simulation will use the interaction’s current linear velocity.

`angularVelocity`  

The angular velocity the toss begins with. If nil, the simulation will use the interaction’s current angular velocity.

## See Also

### Performing actions

protocol Delegate

A protocol for objects that manage the entire flow of players interacting with equipment.

func addAction(some TabletopAction)

func addActions(some Sequence&lt;any TabletopAction>)

func end()

Ends the current interaction.

func cancel()

Cancels the current interaction. All actions added to the interaction will also be cancelled.

