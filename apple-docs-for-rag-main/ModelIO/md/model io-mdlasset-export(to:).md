

- Model I/O
- MDLAsset
-  export(to:) 

Instance Method

# export(to:)

Writes asset data to a file at the specified URL and reports errors that occur during export.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func export(to URL: URL) throws
```

## Parameters 

`URL`  

A URL specifying the location to export asset data to. This parameter must be a `file:` URL.

## Discussion

The MDLAsset class infers the data format to export in from the pathExtension property of the specified URL. To determine whether a format is supported for export, call the canExportFileExtension(_:) method.

## See Also

### Exporting an Asset

class func canExportFileExtension(String) -> Bool

Returns a Boolean value that indicates whether the MDLAsset class can write asset data as a file with the specified format extension.

