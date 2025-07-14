

- RoomPlan
- CapturedRoom
- CapturedRoom.USDExportOptions
-  model 

Type Property

# model

An export option that formats the output file as a collection of 3D models.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static let model: CapturedRoom.USDExportOptions
```

## Discussion

This export option works in conjunction with the CapturedRoomAttribute and CapturedRoom.ModelProvider APIs to replace objects the framework identifies as of a particular category, or to have particular attributes, with 3D models that you choose in advance.

## See Also

### Choosing an export option

static let parametric: CapturedRoom.USDExportOptions

An export option that formats the output file as a collection of size-dependent primitives.

static let mesh: CapturedRoom.USDExportOptions

An export option that formats the output file as a collection of size-independant triangles that connect to form a mesh.

