

- AVFoundation
- AVAssetExportSession
-  exportAsynchronously(completionHandler:) Deprecated

Instance Method

# exportAsynchronously(completionHandler:)

Starts the asynchronous execution of an export session.

iOS 4.0–18.0DeprecatediPadOS 4.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func exportAsynchronously(completionHandler handler: @escaping () -> Void)
```

``` source
func export() async
```

Deprecated

Use export(to:as:isolation:) instead.

## Parameters 

`handler`  

A callback the system invokes when it finishes successfully, or in the event of writing failure.

## See Also

### Exporting Media

func export(to: URL, as: AVFileType, isolation: isolated (any Actor)?) async throws

Exports the asset to the output location in the specified file type.

func cancelExport()

Cancels the execution of an export session.

