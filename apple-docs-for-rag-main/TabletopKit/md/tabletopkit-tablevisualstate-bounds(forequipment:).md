

- TabletopKit
- TableVisualState
-  bounds(forEquipment:) 

Instance Method

# bounds(forEquipment:)

visionOS 2.0+

``` source
func bounds(forEquipment equipment: some Equipment) -> TableVisualState.OrientedRect3D?
```

## See Also

### Representing 3D states

struct OrientedRect3D

An object that represents the position and orientation of a 3D rectangle.

func bounds(matching: EquipmentIdentifier) -> TableVisualState.OrientedRect3D?

func goalBounds(forEquipment: some Equipment) -> TableVisualState.OrientedRect3D?

func goalBounds(matching: EquipmentIdentifier) -> TableVisualState.OrientedRect3D?

var tableBounds: TableVisualState.OrientedRect3D?

