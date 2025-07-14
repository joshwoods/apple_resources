

- AVFoundation
- AVAssetExportSession
-  export(to:as:isolation:) 

Instance Method

# export(to:as:isolation:)

Exports the asset to the output location in the specified file type.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func export(
    to url: URL,
    as fileType: AVFileType,
    isolation: isolated (any Actor)? = #isolation
) async throws
```

## Parameters 

`url`  

An output location to write the exported media. You can use the preferredFilenameExtension property of UTType to determine an appropriate file extension for the specified file type.

`fileType`  

The type of file for the session to write.

`isolation`  

The isolation context.

## Discussion

This method throws an error if you cancel the export or you specify a file type value that isn’t contained in the session’s supportedFileTypes.

You can monitor the status of an export by calling the states(updateInterval:) method.

Note

You can cancel an in-progress export by calling cancel() on the Task or parent task that initiated the operation.

## See Also

### Exporting Media

func cancelExport()

Cancels the execution of an export session.

func exportAsynchronously(completionHandler: () -> Void)

Starts the asynchronous execution of an export session.

Deprecated

