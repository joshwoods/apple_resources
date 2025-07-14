

- TabletopKit
- TabletopGame
-  startInteraction(onEquipmentID:) 

Instance Method

# startInteraction(onEquipmentID:)

Starts a local interaction. It will return `nil` if too many interactions are already happening at the same time.

visionOS 2.0+

``` source
func startInteraction(onEquipmentID equipmentID: EquipmentIdentifier) -> TabletopInteraction.Identifier?
```

