

- TabletopKit
- TableVisualState
-  TableVisualState.OrientedRect3D 

Structure

# TableVisualState.OrientedRect3D

An object that represents the position and orientation of a 3D rectangle.

visionOS 2.0+

``` source
struct OrientedRect3D
```

## Topics

### Creating 3D rectangle states

init()

init(pose: Pose3D, size: Size3D)

init(rotation: Rotation3D, rect: Rect3D)

### Getting 3D rectangle properties

var pose: Pose3D

The pose of the rectangle.

var size: Size3D

The size of the rectangle.

### Default Implementations

Decodable Implementations

Encodable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Representing 3D states

func bounds(forEquipment: some Equipment) -> TableVisualState.OrientedRect3D?

func bounds(matching: EquipmentIdentifier) -> TableVisualState.OrientedRect3D?

func goalBounds(forEquipment: some Equipment) -> TableVisualState.OrientedRect3D?

func goalBounds(matching: EquipmentIdentifier) -> TableVisualState.OrientedRect3D?

var tableBounds: TableVisualState.OrientedRect3D?

