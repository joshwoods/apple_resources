

- RoomPlan
- CapturedRoom
- CapturedRoom.USDExportOptions
-  parametric 

Type Property

# parametric

An export option that formats the output file as a collection of size-dependent primitives.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static let parametric: CapturedRoom.USDExportOptions
```

## Discussion

A parametric model stores elements as unit-sized cubes versus polygonal units. The scale of each element determines whether it appears as a plane or a box.

## See Also

### Choosing an export option

static let mesh: CapturedRoom.USDExportOptions

An export option that formats the output file as a collection of size-independant triangles that connect to form a mesh.

static let model: CapturedRoom.USDExportOptions

An export option that formats the output file as a collection of 3D models.

