

- RoomPlan
- CapturedStructure
-  CapturedStructure.ModelProvider 

Type Alias

# CapturedStructure.ModelProvider

The type a captured structure uses to output sophisticated 3D models.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
typealias ModelProvider = CapturedRoom.ModelProvider
```

## See Also

### Generating a USDZ file

func export(to: URL, metadataURL: URL?, modelProvider: CapturedStructure.ModelProvider?, exportOptions: CapturedStructure.USDExportOptions) throws

Produces a 3D asset from the captured structure.

typealias USDExportOptions

The type a captured structure uses to configure exports.

