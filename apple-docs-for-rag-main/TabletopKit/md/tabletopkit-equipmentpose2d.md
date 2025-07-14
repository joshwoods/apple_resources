

- TabletopKit
-  EquipmentPose2D 

Structure

# EquipmentPose2D

An object that represents the position and rotation of equipment on the XZ plane.

visionOS 2.0+

``` source
struct EquipmentPose2D
```

## Topics

### Creating an equipment pose object

init(id: EquipmentIdentifier, pose: TableVisualState.Pose2D)

Creates a position and rotation on the table for a specific piece of equipment.

### Getting equipment pose properties

var id: EquipmentIdentifier

The unique identifier for the equipment.

var pose: TableVisualState.Pose2D

The 2D position and rotation of equipment on the table.

## Relationships

### Conforms To

- Sendable

## See Also

### Equipment layout

protocol EquipmentLayout

A protocol for objects that describe the layout of equipment.

struct DefaultEquipmentLayout

An object that provides a standard configuration for equipment layout.

struct EquipmentPose3D

An object that represents the 3D position and orientation of equipment on the table.

