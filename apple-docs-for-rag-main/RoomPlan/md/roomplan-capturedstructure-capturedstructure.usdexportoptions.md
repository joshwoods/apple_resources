

- RoomPlan
- CapturedStructure
-  CapturedStructure.USDExportOptions 

Type Alias

# CapturedStructure.USDExportOptions

The type a captured structure uses to configure exports.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
typealias USDExportOptions = CapturedRoom.USDExportOptions
```

## See Also

### Generating a USDZ file

func export(to: URL, metadataURL: URL?, modelProvider: CapturedStructure.ModelProvider?, exportOptions: CapturedStructure.USDExportOptions) throws

Produces a 3D asset from the captured structure.

typealias ModelProvider

The type a captured structure uses to output sophisticated 3D models.

