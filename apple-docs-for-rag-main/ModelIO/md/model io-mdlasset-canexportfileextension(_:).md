

- Model I/O
- MDLAsset
-  canExportFileExtension(\_:) 

Type Method

# canExportFileExtension(\_:)

Returns a Boolean value that indicates whether the MDLAsset class can write asset data as a file with the specified format extension.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class func canExportFileExtension(_ extension: String) -> Bool
```

## Parameters 

`extension`  

The filename extension identifying an asset file format.

## Return Value

true if the MDLAsset class can export asset data in the format with the specified extension; otherwise, false.

## Discussion

If this method returns true, you can use the export(to:) method to write an asset to a file using the format identified by the specified extension.

The set of supported formats includes Wavefront Object (`.obj`) and Standard Tessellation Language (`.stl`). Additional formats may be supported as well.

## See Also

### Exporting an Asset

func export(to: URL) throws

Writes asset data to a file at the specified URL and reports errors that occur during export.

