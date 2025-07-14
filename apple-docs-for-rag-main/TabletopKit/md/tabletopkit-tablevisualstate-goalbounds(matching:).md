

- TabletopKit
- TableVisualState
-  goalBounds(matching:) 

Instance Method

# goalBounds(matching:)

visionOS 2.0+

``` source
func goalBounds(matching equipmentID: EquipmentIdentifier) -> TableVisualState.OrientedRect3D?
```

## See Also

### Representing 3D states

struct OrientedRect3D

An object that represents the position and orientation of a 3D rectangle.

func bounds(forEquipment: some Equipment) -> TableVisualState.OrientedRect3D?

func bounds(matching: EquipmentIdentifier) -> TableVisualState.OrientedRect3D?

func goalBounds(forEquipment: some Equipment) -> TableVisualState.OrientedRect3D?

var tableBounds: TableVisualState.OrientedRect3D?

