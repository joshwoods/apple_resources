

- TabletopKit
-  EquipmentPose3D 

Structure

# EquipmentPose3D

An object that represents the 3D position and orientation of equipment on the table.

visionOS 2.0+

``` source
struct EquipmentPose3D
```

## Topics

### Creating an equipment pose object

init(id: EquipmentIdentifier, pose: Pose3D)

Creates a position and orientation on the table for a specific piece of equipment.

### Getting equipment pose properties

var id: EquipmentIdentifier

var pose: Pose3D

The 3D position and orientation of equipment on the table.

## Relationships

### Conforms To

- Sendable

## See Also

### Equipment layout

protocol EquipmentLayout

A protocol for objects that describe the layout of equipment.

struct DefaultEquipmentLayout

An object that provides a standard configuration for equipment layout.

struct EquipmentPose2D

An object that represents the position and rotation of equipment on the XZ plane.

