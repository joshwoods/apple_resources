

- TabletopKit
- TabletopInteraction
-  cancel() 

Instance Method

# cancel()

Cancels the current interaction. All actions added to the interaction will also be cancelled.

visionOS 2.0+

``` source
func cancel()
```

## See Also

### Performing actions

protocol Delegate

A protocol for objects that manage the entire flow of players interacting with equipment.

func addAction(some TabletopAction)

func addActions(some Sequence&lt;any TabletopAction>)

func toss(equipmentID: EquipmentIdentifier, as: TossableRepresentation, linearVelocity: Vector3D?, angularVelocity: Vector3D?)

Begins a simulation of a toss of the equipment with the specificied parameters. Equipment that begins a toss in the same TabletopInteraction may interact with each other as well as the game’s boundary.

func end()

Ends the current interaction.

