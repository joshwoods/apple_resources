

- AVFoundation
- AVAssetExportSession
- AVAssetExportSession.State
-  AVAssetExportSession.State.exporting(progress:) 

Case

# AVAssetExportSession.State.exporting(progress:)

An export session is currently exporting media.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
case exporting(progress: Progress)
```

## Parameters 

`progress`  

A value that indicates the completion percentage of the export operation.

## See Also

### States

case pending

An export operation is currently pending.

case waiting

An export session is currently waiting.

