

- TabletopKit
-  EquipmentLayout 

Protocol

# EquipmentLayout

A protocol for objects that describe the layout of equipment.

visionOS 2.0+

``` source
protocol EquipmentLayout
```

## Topics

### Laying out equipment

static func planarOverlapping(layout: [EquipmentPose2D], animationDuration: Double?) -> Self

Use the overlapping layout to provide 2d poses for the immediate children and let TabletopKit determine their height and pitch/roll.

static func planarStacked(layout: [EquipmentPose2D], animationDuration: Double?) -> Self

Use the stacked layout to provide 2d poses for the immediate children and let TabletopKit determine their height.

static func volumetric(layout: [EquipmentPose3D], animationDuration: Double?) -> Self

Use the volumetric layout to provide 3d poses for the immediate children directly.

## Relationships

### Conforming Types

- DefaultEquipmentLayout

## See Also

### Equipment layout

struct DefaultEquipmentLayout

An object that provides a standard configuration for equipment layout.

struct EquipmentPose2D

An object that represents the position and rotation of equipment on the XZ plane.

struct EquipmentPose3D

An object that represents the 3D position and orientation of equipment on the table.

