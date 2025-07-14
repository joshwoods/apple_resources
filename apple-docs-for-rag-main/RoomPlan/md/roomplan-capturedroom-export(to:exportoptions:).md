

- RoomPlan
- CapturedRoom
-  export(to:exportOptions:) 

Instance Method

# export(to:exportOptions:)

Produces a 3D asset from the captured room.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func export(
    to url: URL,
    exportOptions: CapturedRoom.USDExportOptions = .mesh
) throws
```

## Parameters 

`url`  

A location that the captured room exports to.

`exportOptions`  

Options that determine the export’s data format.

## Discussion

The file format of the output is Universal Scene Description (USD).

Tip

Before iOS 17.4, the first letter of the USD file name needs to be a character other than a number.

## See Also

### Generating a USDZ file

func export(to: URL, metadataURL: URL?, modelProvider: CapturedRoom.ModelProvider?, exportOptions: CapturedRoom.USDExportOptions) throws

Produces a 3D asset from the captured room with the given metadata output URL and model provider.

struct USDExportOptions

Options that determine the underlying data format of a scan export.

struct ModelProvider

A structure that assigns detailed 3D models to captured objects for an export.

