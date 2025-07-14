

- TabletopKit
- EquipmentLayout
-  volumetric(layout:animationDuration:) 

Type Method

# volumetric(layout:animationDuration:)

Use the volumetric layout to provide 3d poses for the immediate children directly.

visionOS 2.0+

``` source
static func volumetric(
    layout: [EquipmentPose3D],
    animationDuration: Double? = nil
) -> Self
```

Available when `Self` is `DefaultEquipmentLayout`.

## Parameters 

`layout`  

An array of id and 3d pose for each child.

`animationDuration`  

The duration of the transition between the current pose and the new pose. If zero or less than zero the new pose will be applied instantly. If not specified a default duration will be used. If the layout contains poses for equipment that are not immediate children, those poses will be ignored. If the pose of some immediate children is not provided, the previous pose and duration will be used if available.

## See Also

### Laying out equipment

static func planarOverlapping(layout: [EquipmentPose2D], animationDuration: Double?) -> Self

Use the overlapping layout to provide 2d poses for the immediate children and let TabletopKit determine their height and pitch/roll.

static func planarStacked(layout: [EquipmentPose2D], animationDuration: Double?) -> Self

Use the stacked layout to provide 2d poses for the immediate children and let TabletopKit determine their height.

