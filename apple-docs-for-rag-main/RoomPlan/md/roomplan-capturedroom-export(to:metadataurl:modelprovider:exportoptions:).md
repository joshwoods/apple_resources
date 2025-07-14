

- RoomPlan
- CapturedRoom
-  export(to:metadataURL:modelProvider:exportOptions:) 

Instance Method

# export(to:metadataURL:modelProvider:exportOptions:)

Produces a 3D asset from the captured room with the given metadata output URL and model provider.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
func export(
    to url: URL,
    metadataURL: URL? = nil,
    modelProvider: CapturedRoom.ModelProvider? = nil,
    exportOptions: CapturedRoom.USDExportOptions = .mesh
) throws
```

## Parameters 

`url`  

A location that the captured room exports to.

`metadataURL`  

A location that the captured room metadata exports to.

`modelProvider`  

A collection of mappings of object categories and attributes to 3D model URLs.

`exportOptions`  

Options that determine the export’s data format.

## Discussion

The file format of the output is Universal Scene Description (USD).

Tip

Before iOS 17.4, the first letter of the USD file name needs to be a character other than a number.

## See Also

### Generating a USDZ file

func export(to: URL, exportOptions: CapturedRoom.USDExportOptions) throws

Produces a 3D asset from the captured room.

struct USDExportOptions

Options that determine the underlying data format of a scan export.

struct ModelProvider

A structure that assigns detailed 3D models to captured objects for an export.

