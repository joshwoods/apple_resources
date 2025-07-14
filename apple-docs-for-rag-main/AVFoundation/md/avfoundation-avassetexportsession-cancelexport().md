

- AVFoundation
- AVAssetExportSession
-  cancelExport() 

Instance Method

# cancelExport()

Cancels the execution of an export session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7–11.0DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0+

``` source
func cancelExport()
```

## Discussion

Apple discourages the use of this symbol. Use cancel() on the Task or parent task that initiated the export instead.

## See Also

### Exporting Media

func export(to: URL, as: AVFileType, isolation: isolated (any Actor)?) async throws

Exports the asset to the output location in the specified file type.

func exportAsynchronously(completionHandler: () -> Void)

Starts the asynchronous execution of an export session.

Deprecated

